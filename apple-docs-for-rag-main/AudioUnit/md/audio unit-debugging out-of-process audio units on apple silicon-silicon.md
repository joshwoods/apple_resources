

- Audio Unit
-  Debugging Out-of-Process Audio Units on Apple Silicon 

Article

# Debugging Out-of-Process Audio Units on Apple Silicon

Connect to out-of-process audio units using the Xcode debugger.

## Overview

Beginning with macOS 11, the system loads audio units into a separate process that depends on the architecture or host preference. This increases stability and security by isolating audio units from their host app, and allows loading x86 audio units into an Apple silicon host app.

Attaching to system processes requires disabling system integrity protection in macOS before debugging. For more information, see Disabling and Enabling System Integrity Protection.

### Attach to the Hosting Service

After disabling system integrity protection, follow these steps to debug an out-of-process audio unit in Xcode:

1.  Build and run an app to install it.

2.  Stop the debugging session by choosing Product \> Stop.

3.  Choose Debug \> Attach to Process by Name.

4.  Enter the process name `AUHostingServiceXPC` or `AUHostingServiceXPC_arrow.`

5.  Click the Attach button to begin debugging.

The process name to use depends on the host, as well as the architectures of the host and plugin. There are currently two process names — `AUHostingServiceXPC_arrow` for Rosetta and `AUHostingServiceXPC` for native — and they may change in future updates.

Warning

Leaving system integrity protection in a disabled state makes your computer vulnerable to malicious code, so enable it when you finish debugging your audio units.

### Troubleshoot Common Issues for Audio Units

Debugging is generally a seamless process, but if you encounter issues, consider the following:

- When setting audio unit properties, don’t assume callbacks happen on the main thread. When updating the user interface, asynchronously dispatch to the main queue.

- The differences in the way mouse-tracking APIs work can lead to processing mouse events in unexpected ways, so use event deltas for calculations that involve mouse movement.

- If custom, free-floating dialogs don’t work as you expect, add them as a subwindow to the main window — this includes custom tooltip and drop-down menu implementations.

- Because an audio unit and its host app operate within separate processes, you can’t create custom properties that share pointers to objects. The Core Audio framework must handle this, so if you have a specific need, submit a feedback request.

