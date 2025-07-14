

- Core Media I/O
-  Creating a camera extension with Core Media I/O 

Article

# Creating a camera extension with Core Media I/O

Build high-performance camera drivers that are secure and simple to deploy.

## Overview

Camera extensions are a new type of system extension available in macOS 12.3 and later. They provide a simple, secure model for building high-performance camera drivers for macOS. You package and install them with your app, which makes them simple to deploy, including through the App Store.

Related Sessions from WWDC22

Session 10022: Create camera extensions with Core Media I/O

The following illustration shows a high-level view of a camera extension.

A camera extension consists of three primary components:

- A CMIOExtensionProvider represents the primary interface to the extension. The provider and its source manage the extension’s device and client connections, and also define properties common to the extension such as its name and manufacturer.

- A CMIOExtensionDevice represents a hardware or software device that the extension publishes as a selectable camera in apps like FaceTime. A device and its source configure supporting resources like buffer pools that it uses when streaming data. A device also defines properties for values such as its model name and transport type.

- A CMIOExtensionStream represents a stream of data to send to clients. A stream and its source specify the stream’s format, minimum and maximum frame rates, and direction. A stream’s source object is responsible for starting and stopping the stream’s flow of data.

To simplify creating your own extensions, Xcode provides a Camera Extension template that provides a fully functional extension implementation. It creates a virtual camera device that renders a horizontal white line that moves up and down the display. This article shows how to configure the template’s output to build your own camera extension.

Note

See the System Extensions framework for additional information on building, installing, and debugging system extensions.

### Add entitlements to your host app

You package your camera extension as part of your app bundle. To allow your app to install and communicate with the extension, your app target requires two additional capabilities. Select the target in Xcode, and click the Signing & Capabilities pane. Add the following capabilities to the target:

- System Extension. This capability enables the app to install system extensions.

- App Groups. This capability enables the app to define a common group container for the app and the extension to share, which allows them to communicate.

Adding the capabilities to the target writes the values to an entitlements file. For example, an app with a bundle identifier of `com.example.CustomCamera` would have an entitlements file similar to the following:

```
```

### Create a camera extension target

Add a new target to your app using the Camera Extension template. In Xcode, go to the File menu and choose File \> New and select the Target menu item. In the dialog that appears, select the macOS pane and find the Camera Extension template as shown below.

Click the Next button. On the screen that follows, give the extension an appropriate name and leave the other values set to their defaults, and then click the Finish button.

The template creates a new target and folder with the name you specified. The folder contains the following files:

- A `[CameraExtensionName]Provider.swift` file that provides the complete extension implementation.

- A `main.swift` file that provides the minimal code for the system to initialize the extension.

- An `Info.plist` that defines the `CMIOExtensionMachServiceName` for the extension and a NSSystemExtensionUsageDescriptionKey that describes the extension’s purpose to the user.

- A `[CameraExtensionName].entitlements` file that defines a default app group.

### Configure the extension

So that your app and extension can communicate, open the `[CameraExtensionName].entitlements` file and update it to use the same app group name that you defined in your app, as in the example below.

```
```

Next, open the `[CameraExtensionName]Provider.swift` file. This file provides a complete implementation for all components of a camera extension. Look through the file and familiarize yourself with the code.

You can quickly find essential user-customizable strings by searching the file for the string, `SampleCapture`, and replacing the values as appropriate. A particularly important string to customize is the localizedName that you specify for the CMIOExtensionDevice, because it’s the string that apps display in their camera selection UI.

### Activate the extension

The system automatically installs a camera extension when a user installs your app. However, before your extension is available for the system to use, your app needs to activate it by performing an activation request like shown below.

```
```

Only apps that reside in the `/Applications` directory can activate an extension. To test your extension, move your app from Xcode’s build results to the `/Applications` folder. Launch your app from its new location to test its activation request. When it attempts to activate the extension, the system prompts the user with a dialog like shown below.

Before the extension is available to the system, a person with Admin privileges for the Mac must explicitly allow access to it in the Systems & Privacy screen of System Settings.

Tip

During development of your extension, it’s often useful to temporarily disable some security restrictions imposed by the system. See Debugging and testing system extensions for more information.

### Access the custom camera

After you’ve allowed the system to use your custom extension, it’s automatically available as a selectable camera in system apps like FaceTime and PhotoBooth. Camera extensions are also fully compatible with AVFoundation capture APIs, which means you can access your extension as an AVCaptureDevice object and use it like any other device. For example, to retrieve your custom camera extension (as well as any others on the system), retrieve it as an externalUnknown device type as shown below.

```
```

## See Also

### Providers

Overriding the default USB video class extension

Create a simple DriverKit extension to override the default driver-matching behavior for USB devices.

class CMIOExtensionProvider

An object that manages device connections for a provider.

protocol CMIOExtensionProviderSource

A protocol for objects that act as provider sources.

class CMIOExtensionProviderProperties

An object that manages the properties of an extension provider.

