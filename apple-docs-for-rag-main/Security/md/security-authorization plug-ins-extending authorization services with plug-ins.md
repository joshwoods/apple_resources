

- Security
- Authorization Plug-ins
-  Extending authorization services with plug-ins 

Article

# Extending authorization services with plug-ins

Modify the system’s authorization policy with custom code.

## Overview

Important

To authenticate the person using your app prior to providing access to resources within the app, use Local Authentication instead of creating an authorization plug-in. Use authorization plug-ins to extend or change system policies.

The macOS Security Server’s authorization engine consults its authorization policy database to determine which authorization mechanisms to use when evaluating whether to grant particular rights for the person using the Mac. You can customize this process by creating an authorization plug-in, a code bundle that provides one or more authorization mechanisms. Each authorization mechanism performs a single step in an authorization process.

If the policy database specifies a mechanism in your authorization plug-in, the authorization engine loads your plug-in in a dedicated host process to isolate your code. There are two plug-in hosts:

- One that runs as an anonymous user and can communicate with the user; for example, to ask for a password.

- One that runs with root privileges to perform privileged operations.

Important

Authorization plug-ins that display an interface or otherwise connect to the window server can’t run in the privileged plug-in host. Running GUI code as root is — in general — a bad idea because GUI code links in many libraries, any of which could contain security vulnerabilities.

### Create an authorization plug-in

The entry point for your authorization plug-in is the AuthorizationPluginCreate function. Your implementation of this function receives the Security Server’s authorization interface functions in an AuthorizationCallbacks structure, and passes the plug-in’s interface to the Security Server by populating the AuthorizationPluginInterface structure.

Call the SetResult function to report the authorization decision.

Communicate auxiliary information by setting and getting *hints* and *context data*. Hints are data values for use during authorization; for example, you can use a hint to pass an intermediate value from one mechanism to a subsequent mechanism. Hints aren’t preserved as part of the authorization result. You set hints by calling SetHintValue, and retrieve them by calling GetHintValue.

Context data is information that can be useful to an application, such as a user name the person enters during the authorization process. Each mechanism in the authorization can add, read, or modify context data, which the Security Server preserves. The Security Server can also make context data available to the authorization client when authorization is complete. You set context data by calling SetContextValue, and retrieve them by calling GetContextValue.

When you set context data, tag the data with a flag that specifies whether the Security Server should return the data to the authorization client upon request (by using the AuthorizationCopyInfo(_:_:_:) function), or whether it’s restricted to the mechanisms involved in the authorization.

Important

If your plug-in displays a window before somebody logs into a Mac, ensure you set the canBecomeVisibleWithoutLogin property of your NSWindow instance to true. For more details, see AuthorizationPluginCreate.

### Register the authorization plug-in

To install an authorization plug-in so that the authorization engine can find it and use its authorization mechanisms, copy the bundle to `/Library/Security/SecurityAgentPlugins` as part of your app’s installation process. In your app, call AuthorizationRightSet(_:_:_:_:_:_:) to add a rule to the authorization policy database that refers to your plug-in. Pass a dictionary as the `rightDefinition` parameter, using the keys listed in Authorization Name Tags and those in the file `AuthorizationTagsPriv.h`.

Important

`AuthorizationTagsPriv.h` isn’t part of the public API. Apple reserves the right to change this file or its contents with future releases.

The name of a mechanism is the plug-in name, followed by a colon (`:`), and the name of the mechanism. To indicate that the authorization engine should load the plug-in in the privileged host, add a comma and the word `privileged` to the mechanism name; for example:

```
SendFaxPlugin:ChangeUserPIN,privileged
```

### Participate in authorization decisions

When the authorization engine needs an authorization decision based on a policy defined in the policy database, it calls each mechanism belonging to that policy in turn, in the order they’re listed in the policy database. For each mechanism, the authorization engine calls the plug-in’s MechanismInvoke function, passing the plug-in `name:mechanism` string for that mechanism.

The authorization engine doesn’t consider the authorization complete and approved until all mechanisms call SetResult to return a positive authorization decision (kAuthorizationResultAllow), one of the mechanisms calls SetResult to return a negative decision (kAuthorizationResultDeny), the maximum number of retries is reached (kAuthorizationResultUndefined), or the person cancels the attempt (kAuthorizationResultUserCanceled).

### Request an authorization decision

To discover the outcome of an authorization decision based on a policy that refers to your plug-in’s mechanisms, you don’t call your plug-in’s code directly. Instead, you call AuthorizationCopyRights(_:_:_:_:_:), passing the name of the policy that references that plug-in in the rights parameter. The authorization engine uses a hierarchical strategy to find a rule matching the requested policy name. For example, if your app requests the `com.example.myProduct.transcripts.create` right, then the authorization searches for these rules in order:

1.  `com.example.myProduct.transcripts.create`

2.  `com.example.myProduct.transcripts.`

3.  `com.example.myProduct.`

4.  `com.example.`

5.  `com.`

6.  A generic rule, that’s always present.

The default policy for the generic rule is to require that the person authenticate as a member of the `admin` group. The Security Server can share successful authentication with multiple apps, with a timeout of 300 seconds.

