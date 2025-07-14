

- Technotes
-  TN3113: Testing and debugging XPC code with an anonymous listener 

Article

# TN3113: Testing and debugging XPC code with an anonymous listener

Use an anonymous XPC listener to simplify your XPC testing and debugging.

## Overview

Testing and debugging XPC code is tricky because there are two processes involved. Imagine you have an app with an embedded XPC service. To debug this you have to run two instances of the debugger, one connected to the app and another to the service, and then switch between them. This works, but it’s quite inconvenient. Fortunately there is a better way, a technique that allows you to test and debug all your XPC code in a single process.

Important

This technique does not help with all XPC testing and debugging scenarios. For example, if you’re developing a `launchd` daemon that performs privileged operations on behalf of your app, you can’t use this technique to debug your privileged code because it’s not running in a privileged process. However, even in situations like that, this technique is useful when debugging your XPC-specific code. For example, you might use it to create a unit test for your NSSecureCoding implementation.

This technique involves two key concepts:

- Put your XPC listener and XPC client code in the same test program. The specifics of this program are up to you: It might be a simple test app that you create specifically for this purpose, or it might be an Xcode unit test bundle, or it might be some other kind of program.

- Use an anonymous XPC listener to connect your XPC listener and client code.

Imagine you’re building an app with an embedded XPC service. You have a `MyListener` class that manages your XPC listener within the XPC service, and a `MyConnection` class that manages the connection on the app side of things. Add both of those classes, and all their support code, to your test program. Then change `MyListener` to accept an `NSXPCListener` instance. For example, your `MyListener` class might look like this:

```
class MyListener {

    init() {
        self.listener = NSXPCListener.service()
    }

    let listener: NSXPCListener

    … more code …
}
```

Note

While this example uses the Foundation XPC API, the same technique works for the low-level C XPC API.

Change its initialiser to look like this:

```
init(listener: NSXPCListener = .service()) {
    self.listener = listener
}
```

This uses the XPC service’s listener by default, but allows you to override that by passing in a value to the `listener` parameter.

Now, in your test program, call anonymous() to create a anonymous listener and pass that to your listener abstraction:

```
let myListener = MyListener(listener: .anonymous())
```

On the client side, your `MyConnection` class might look like this:

```
class MyConnection {

    init() {
        self.connection = NSXPCConnection(serviceName: "com.example.MyService")
    }

    let connection: NSXPCConnection
}
```

Change the initialiser to look like this:

```
init(connection: NSXPCConnection = .init(serviceName: "com.example.MyService")) {
    self.connection = connection
}
```

This sets up a connection to the XPC service’s listener by default, but allows you to override that by passing in a value to the `connection` parameter.

Finally, in your test program, use init(listenerEndpoint:) to create a connection to your anonymous listener:

```
let connection = NSXPCConnection(listenerEndpoint: myListener.listener.endpoint)
let myConnection = MyConnection(connection: connection)
```

You now have an XPC connection between your client code and your listener, with all the code running in the same test program. This makes it much easier to debug your XPC code. And the same technique is perfect for unit tests.

## Revision History

- **2022-04-12** Added syntax highlighting to the code listings (r. 89366505).

- **2022-02-08** Republished as TN3113. Expanded the introduction to clarify the overall concept. Made other minor editorial changes.

- **2021-11-09** First published as ”Testing and Debugging XPC Code With an Anonymous Listener” on Apple Developer Forums.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

