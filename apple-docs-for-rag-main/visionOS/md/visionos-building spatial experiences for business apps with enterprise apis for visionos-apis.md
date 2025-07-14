

- visionOS
-  Building spatial experiences for business apps with enterprise APIs for visionOS 

Article

# Building spatial experiences for business apps with enterprise APIs for visionOS

Grant enhanced sensor access and increased platform control to your visionOS app by using entitlements.

## Overview

Note

This article is associated with WWDC24 session 10139: Introducing enterprise APIs for visionOS.

You can use the entitlements that enterprise APIs for visionOS offer to create even more powerful enterprise solutions and spatial experiences for your visionOS app. The enterprise APIs for visionOS consist of two distinct categories.

The first category of APIs provides enhanced sensor access and improves the visual capabilities of Apple Vision Pro, including access to the main camera, improved capture and streaming, and enhanced functionality through the camera that allows you to see what the wearer sees.

Main camera access  
Capture input data from the forward-facing main camera.

Passthrough in screen capture  
Access a composite feed of what an Apple Vision Pro wearer is seeing (physical world and digital content).

Spatial barcode and QR code scanning  
Scan barcodes and QR codes with the ability to decode contents and locate spatial positions.

The second category focuses on platform control to help you get the most out of visionOS. These entitlements provide advanced machine learning (ML) capabilities using the Apple Neural Engine for your custom ML model, enhanced object-tracking capabilities for faster object detection, and the ability to tune the performance of your apps to achieve even more compute functionality for intensive workloads.

Apple Neural Engine access  
Specifically target Apple Neural Engine (ANE) for machine learning tasks, similar to iOS.

Object-tracking parameter adjustment  
Optimize known object detection and tracking using configurable parameters.

Increased performance headroom  
Use increased power of the CPU and GPU for high-compute needs, with a tradeoff of increased thermal usage and reduced battery life.

UVC Device Access on visionOS  
Stream USB UVC devices connected to the Developer strap.

Note

Each of these entitlements allows a device to operate outside the default configuration. When using these features, be aware that they may impact the performance of other apps.

### Request the entitlements

If you’re interested in using the enterprise APIs for visionOS in your app, the Account Holder of your Apple Developer Program and/or Apple Developer Enterprise Program can submit an entitlement request.

To be eligible, your app needs to:

- Be for use in a business setting only

- Meet specific criteria associated with usage for each API

Enterprise APIs for visionOS are eligible for business use only. You can distribute apps that you develop with the enterprise APIs for visionOS privately as proprietary in-house apps or custom apps using Apple Business Manager. For more information on distributing custom apps, see Set distribution methods.

You can also request access to the entitlements for *Development Only* purposes. With this access, you can build and run apps on your registered test devices with development provisioning profiles.

### Configure your app’s Xcode project

To use entitlements, you need to include both the entitlement file and a corresponding license file in your app. After Apple approves your app for one or more entitlements, you receive a license file, along with additional instructions.

You add the license file to your app’s Xcode project. Placing the license file within your project and adding it to your build target allows Xcode to compile it within your app and then validate it when checking your entitlements.

Note

The license file comes with an expiration date, so you need to renew it before then to ensure your entitlements continue to function.

To add an entitlement in Xcode:

1.  Select your project in the Project navigator.

2.  Select the applicable target and then click the Signing & Capabilities tab.

3.  Click the Add Capability button (+) and type the name of the entitlement you want to add, such as *main camera access*.

4.  Double-click the entitlement to add it to the Signing section. This creates a `.entitlements` file with the relevant capability, such as `com.apple.developer.arkit.main-camera-access.allow` for “Main camera access”.

After you add the `.license` and `.entitlements` files, you can implement and test the APIs you have approval to use. For more information, see Adding capabilities to your app.

## See Also

### Enterprise APIs for visionOS

Accessing the main camera

Add camera-based features to enterprise apps.

Displaying video from connected devices

Show video from devices connected with the Developer Strap in your visionOS app.

Locating and decoding barcodes in 3D space

Create engaging, hands-free experiences based on barcodes in a person’s surroundings.

