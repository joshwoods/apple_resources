

- Xcode
- Capabilities
-  Configuring the hardened runtime 

Article

# Configuring the hardened runtime

Protect the runtime integrity of your macOS app by restricting access to sensitive resources and preventing common exploits.

## Overview

The *Hardened Runtime* is a collection of system-enforced restrictions that disable a set of functional capabilities, such as loading third-party frameworks, and prohibit access to restricted resources, such as the device’s built-in camera, to prevent certain classes of exploits from compromising the runtime integrity of your macOS app. If your app relies on something the Hardened Runtime restricts, you remove that specific protection by adding an entitlement to your app’s entitlements file. Xcode’s Hardened Runtime capability provides an easy way to manage those entitlements.

Before you select the required runtime exceptions and access to restricted resources that your app requires, follow the steps in the Add a capability section of Adding capabilities to your app to add the Hardened Runtime capability to the target of your macOS app. If you create a new macOS app using a template, Xcode automatically adds the Hardened Runtime capability to your app.

Important

Apple only notarizes macOS apps that enable the Hardened Runtime capability. For more information, see Notarizing macOS software before distribution.

### Specify your app’s runtime exceptions

Before your app can perform functionality that depends upon one or more runtime exceptions, you must add the entitlements for those exceptions by performing the following:

1.  Select your project in Xcode’s Project navigator.

2.  Select the app’s target in the Targets list.

3.  Click the Signing & Capabilities tab in the project editor.

4.  Locate the Runtime Exceptions section of the Hardened Runtime capability.

5.  Select one or more runtime exceptions by checking the corresponding checkboxes.

Xcode automatically updates your app’s entitlements file to include the entitlements that correspond to the selected runtime exceptions, and sets the value of those entitlements to `true`.

The following table describes the runtime exceptions the Hardened Runtime supports:

| Name | Functionality |
|----|----|
| Allow Execution of JIT-compiled Code | Create writable and executable memory using the `MAP_JIT` flag. For more information, see Allow execution of JIT-compiled code entitlement. |
| Allow Unsigned Executable Memory | Create writable and executable memory without the imposed restrictions of the `MAP_JIT` flag. Useful for legacy apps. For more information, see Allow Unsigned Executable Memory Entitlement. |
| Allow DYLD Environment Variables | Modify your app’s behavior at runtime using dynamic link variables. For more information, see Allow DYLD environment variables entitlement. |
| Disable Library Validation | Load frameworks and plug-ins that are written by third-party developers. For more information, see Disable Library Validation Entitlement. |
| Disable Executable Memory Protection | Disable the protections that code-signing provides. For more information, see Disable Executable Memory Protection Entitlement. |
| Debugging Tool | Attach to other processes or get task ports by indicating to the system that your app’s a debugger. For more information, see Debugging tool entitlement. |

Warning

Specific runtime exceptions, such as Disable Executable Memory Protection, remove core security barriers from your app. Always apply caution when using runtime exceptions and opt for the narrowest set of entitlements that enable the required functionality.

### Specify the resource access your app requires

If your app accesses restricted or sensitive resources, such as the user’s photo library or address book, you must include the entitlements that provide access to those resources by following these steps:

1.  Select your project in Xcode’s Project navigator.

2.  Select the app’s target in the Targets list.

3.  Click the Signing & Capabilities tab in the project editor.

4.  Locate the Resource Access section of the Hardened Runtime capability.

5.  Select access to one or more resources by checking the corresponding checkboxes.

After you select the required resource access, Xcode updates the entitlements file of your app to include the corresponding entitlements and sets the value of those entitlements to `true`.

Important

Apps that contain the necessary entitlements must still seek the user’s explicit permission before they can access restricted resources such as the camera. See each resource’s corresponding framework documentation for specific requirements.

The following table describes the resource access entitlements the Hardened Runtime supports:

| Name | Functionality |
|----|----|
| Audio Input | Record audio using the built-in microphone and access audio input using the Core Audio APIs. For more information, see Audio Input Entitlement. |
| Camera | Capture images and movies with the built-in and external cameras. For more information, see Camera entitlement. |
| Location | Determine the user’s location using Location Services. For more information, see Location entitlement. |
| Contacts | Enable read-write access to the user’s Contacts database. For more information, see Address book entitlement. |
| Calendar | Enable read-write access to the user’s calendar. For more information, see Calendars entitlement. |
| Photos Library | Enable read-write access to the user’s photo library. For more information, see Photos Library Entitlement. |
| Apple Events | Post Apple Events to other apps and processes. For more information, see Apple Events Entitlement. |

## See Also

### Security

Configuring the macOS App Sandbox

Protect system resources and user data from compromised apps by restricting access to the file system, network connections, and more.

Configuring keychain sharing

Share keychain items between multiple apps belonging to the same developer.

