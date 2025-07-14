

- visionOS
-  Accessing the main camera 

Sample Code

# Accessing the main camera

Add camera-based features to enterprise apps.

Download

visionOS 2.0+Xcode 16.0+

## Overview

This sample code project demonstrates how to use ARKit to access and display the left main camera frame in your visionOS app. You can use this functionality to implement computer vision-powered experiences or live streaming in your enterprise app. For instance, support technicians can live stream their surroundings to remote experts for improved guidance.

### Configure the sample code project

Replace `Enterprise.license` with your license file. The sample app requires a valid license file to display the main camera.

### Request the entitlement

Main camera access is a part of enterprise APIs for visionOS, a collection of APIs that unlock capabilities for enterprise customers. To use main camera access, you need to apply for the Main camera access entitlement. For more information, including how to apply for this entitlement, see Building spatial experiences for business apps with enterprise APIs for visionOS.

### Add usage descriptions for ARKit data access

To help protect people’s privacy, visionOS limits app access to cameras and other sensors in Apple Vision Pro. You need to add an `NSEnterpriseMCAMUsageDescription` to your app’s information property list to provide a usage description that explains how your app uses the data these sensors provide. People see this description when your app prompts for access to camera data.

Note

In visionOS, ARKit is only available in an immersive space. See Setting up access to ARKit data to learn more about opening an immersive space and requesting authorization for ARKit data access. To learn more about best practices for privacy, see Adopting best practices for privacy and user preferences.

### Access and display main camera frames

The following code example accesses and displays the left main camera at the highest available resolution. To access the camera, start an ARKitSession with a CameraFrameProvider, and then request CameraFrameProvider.CameraFrameUpdates in a given format. ARKit delivers a stream of CameraFrame instances; each frame includes a CameraFrame.Sample containing a pixelBuffer and CameraFrame.Sample.Parameters describing the frame’s characteristics.

```
import ARKit
import RealityKit
import SwiftUI

struct MainCameraView: View {
    @State private var arkitSession = ARKitSession()
    @State private var pixelBuffer: CVPixelBuffer?

    let emptyImage = Image(systemName: "camera")

    var body: some View {
        let image = pixelBuffer?.image ?? emptyImage

        image
        .resizable()
        .scaledToFit()
        .task {

            // Check wether there's support for camera access; otherwise, handle this case.
            guard CameraFrameProvider.isSupported else {
                return
            }

            let cameraFrameProvider = CameraFrameProvider()

            try? await arkitSession.run([cameraFrameProvider])

            // Read the video formats that the left main camera supports.
            let formats = CameraVideoFormat.supportedVideoFormats(for: .main, cameraPositions: [.left])

            // Find the highest resolution format.
            let highResolutionFormat = formats.max { $0.frameSize.height 

To display the frame’s content, convert its pixelBuffer to an Image using the following extension:

```
extension CVPixelBuffer {
    var image: Image? {
        let ciImage = CIImage(cvPixelBuffer: self)
        let context = CIContext(options: nil)

        guard let cgImage = context.createCGImage(ciImage, from: ciImage.extent) else {
            return nil
        }

        let uiImage = UIImage(cgImage: cgImage)

        return Image(uiImage: uiImage)
    }
}
```

## See Also

### Enterprise APIs for visionOS

Building spatial experiences for business apps with enterprise APIs for visionOS

Grant enhanced sensor access and increased platform control to your visionOS app by using entitlements.

Displaying video from connected devices

Show video from devices connected with the Developer Strap in your visionOS app.

Locating and decoding barcodes in 3D space

Create engaging, hands-free experiences based on barcodes in a person’s surroundings.

