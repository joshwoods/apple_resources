

- Xcode
-  Building and running an app 

Article

# Building and running an app

Compile your source files and assemble an app bundle to run on a device or simulator.

## Overview

During development, you build and run an app many times to test new features and eliminate bugs. Each time you build, Xcode analyzes your app’s source files to determine which ones it must recompile. Xcode also identifies any other tasks that it must perform, such as running custom scripts. Depending on the state of your project, Xcode performs either a complete rebuild of everything, or an incremental build of only the changed items.

When you run an app after a successful build, Xcode launches the app on the selected device. Mac apps run on the same device as your Xcode installation. iOS, iPadOS, tvOS, visionOS, and watchOS apps run either on a connected device or in a simulated environment on your Mac.

### Configure a target for your app

Xcode determines how to build apps and other products from your project’s target information. A *target* contains the tasks required to create an executable, and the settings to use to build it. For example, an app target might contain the list of files to compile, the resources to copy into the app’s bundle, and other steps needed to configure the app.

When you create a new project, the template you choose includes a default target, which Xcode configures using the information you provide. You can add new targets to your project at any time to create additional products. For information about how to configure new targets, see Configuring a new target in your project.

### Select a scheme for your target

A *build scheme* is a collection of settings that specify which targets to build, the build configuration to use, and the executable environment for the running product. Xcode creates schemes for most targets automatically, and you can create additional schemes to customize the build and execution options. For example, you might create a new scheme to pass additional launch arguments to your app.

To build an app, or any other target, select a scheme that contains the target. Xcode displays the selected scheme in the toolbar of your project window. To change the selected scheme, click the scheme name and choose a new one from the pop-up menu.

For information about how to configure your project’s schemes, see Customizing the build schemes for a project.

### Tell Xcode where to run your app

When you select a scheme to build, you also select a destination where you run the built products. Each scheme contains a list of real or simulated devices that represent the available destinations. To select a destination, click the destination name, which is next to the scheme name in the toolbar. Select an appropriate device from the pop-up menu.

Choose a destination that gives you the capabilities you need. For Mac products, select My Mac. For other platforms, if the app doesn’t require actual hardware, you can choose a simulator to test features quickly on your Mac. If your app requires actual hardware, or you’re ready to see how your app behaves in real conditions, select a real device. For information on configuring new simulated devices or connecting to a real device, see Running your app in Simulator or on a device.

Important

Before you ship any code, test and gather metrics on real devices. Simulators offer quick turnaround times during development, but they don’t simulate the actual performance of target devices.

### Build, run, and debug your app

To build and run your code, choose Product \> Run, or click the Run button in your project’s toolbar.

Xcode analyzes your scheme’s targets and builds them in the proper sequence. After a successful build, Xcode launches the associated app. If you enabled the Debug executable option in your scheme, Xcode attaches the debugger to the app immediately after launch. To build a scheme without running the app, select Product \> Build instead.

If Xcode encounters an error during a build, Xcode reports the error in the Issue navigator and stops. If you enable the “Continue building after errors” setting in the General tab of Xcode preferences, Xcode continues to build and report errors for the rest of your project’s files. To stop an in-progress build, select Product \> Stop, or click the Stop button in your project’s toolbar.

A scheme’s build configuration determines how Xcode launches the product. For a scheme that builds an app, Xcode launches the app itself. For other products, you specify the app to launch using the scheme editor. You can also use the scheme editor to specify launch arguments, runtime data, and debugging parameters.

## See Also

### Essentials

Creating an Xcode project for an app

Start developing your app by creating an Xcode project from a template.

Creating your app’s interface with SwiftUI

Develop apps in SwiftUI with an interactive preview that keeps the code and layout in sync.

Previewing your app’s interface in Xcode

Iterate designs quickly and preview your apps’ displays across different Apple devices.

Xcode updates

Learn about important changes to Xcode.

