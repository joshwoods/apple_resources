

- BrowserEngineKit
- Extension lifecycle
-  Managing the browser extension life cycle 

Article

# Managing the browser extension life cycle

Coordinate helper processes to efficiently support your browser app.

## Overview

When your browser app uses an alternative browser engine, it relies on helper processes to access operating-system resources and work with untrusted resources, following the security principle of least privilege. Use the BrowserEngineKit framework to manage these processes, and notify the operating system of the status of each process as it supports your browser app.

### Launch browser extensions

Your browser app acts as the “host” for each of the extensions that support your browser engine. You need to include the code to launch each extension in your browser app; one extension can’t load another extension.

To launch an extension, your browser app creates and initializes an instance of the structure that represents the running extension process. Pass an *interruption handler* to the initializer, to execute cleanup code if the operating system interrupts the extension process or the extension crashes. For example, to launch a web content extension:

```
let contentProcess = WebContentProcess() {
  // Handle the web content extension getting interrupted.
}
```

To launch the GPU extension, create a RenderingProcess instead of a WebContentProcess. To launch the networking extension, create a NetworkingProcess instead.

### Communicate between your browser app and its extensions

Use the WebContentProcess, RenderingProcess, and NetworkingProcess objects to create inter-process communication (IPC) channels between your host app and the extensions.

For more information, see Using XPC to communicate with browser extensions.

### Put the content extension in a restricted sandbox

The operating system creates a temporary sandbox when it starts your content extension process, which gives the extension access to resources it uses during initialization. For more information: see Limiting resource access in web content extensions.

### Grant and invalidate extension capabilities

As your extensions participate in your browser app’s workflow, grant them capabilities that tell the operating system what your browser is using the extensions for. Capabilities act as assertions to the operating system that it needs to schedule the extension to support particular tasks, for example preparing media content to display in a tab that’s in the foreground on the person’s screen.

You identify the capability to grant to the extension by selecting the appropriate value from the ProcessCapability enumeration. In your browser app, pass the capability to the extension process’s `grantCapability()` method to receive a *grant* object of type ProcessCapability.Grant, indicating that the operating system granted the capability to your extension. When you finish the task that requires the capability, call invalidate() on the grant object to relinquish the capability.

For example, to request and use the ProcessCapability.foreground capability for the networking process:

```
if let grant = try? networkingProcess.grant(.foreground) {
  // Use XPC to send messages to the networking extension while it has the capability.
  grant.invalidate()
} else {
  // The operating system didn't grant the capability to the extension.
}
```

### Stop extension processes

When you no longer need an extension process, call its `invalidate()` method to indicate to the operating system that it can stop the process. Once you have invalidated a process, it’s an error to call other methods on the process object.

## See Also

### Essentials

Using XPC to communicate with browser extensions

Build interprocess communication between your host app and extensions.

