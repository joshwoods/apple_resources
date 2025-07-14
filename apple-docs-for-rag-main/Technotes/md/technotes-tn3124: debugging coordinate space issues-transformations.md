

- Technotes
-  TN3124: Debugging coordinate space issues 

Article

# TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

## Overview

Working with coordinate spaces is an essential part of developing any graphics-based app. Issues related to assumptions or misinterpretations of a coordinate space are difficult to debug, or even identify. Read this technote to discover effective strategies for diagnosing and debugging coordinate space issues.

## Recognize the issue

Coordinate space issues can be difficult to recognize, but there are some common symptoms that can help to diagnose them:

- Unexpected or absent visual appearance

- Incorrect behavior of user-interaction

- Wrong values after a coordinate conversion

Assume that there is a coordinate space issue that needs to be debugged if you notice any of these symptoms in your app.

## Identify the coordinate spaces involved

Coordinate spaces are ubiquitous in the graphics world. Even simple apps will involve many different coordinate spaces. Identifying the coordinate spaces involved is essential to debugging issues with them.

Consider the following SwiftUI snippet:

```
struct ContentView: View {

    @State private var uiImage = UIImage()

    var body: some View {
        VStack {
            Image(uiImage: uiImage)
            Button("Hello") {
                print("World.")
            }
        }
    }
}
```

This snippet, while simple, actually involves five different coordinate spaces:

1.  The local coordinate space of the `VStack`.

2.  The local coordinate space of the `Image`.

3.  The local coordinate space of the `Button`.

4.  The local coordinate space of the `UIImage`.

5.  The global coordinate space of `SwiftUI`.

## Create a focused sample

Coordinate space issues are often very complex and difficult to reason about. Creating a focused sample project that visualizes origins, logs transforms and bounding boxes, and utilizes known points is an extremely effective tool for debugging coordinate space issues.

## Visualize the origin

The best first step towards understanding a coordinate space is to visualize its origin.

Warning

Do not rely on textual descriptions of a coordinate space, they are easy to misinterpret.

Projects targeting visionOS can use Xcodes’s Debug Visualizations. In other contexts, the exact code to visualize the origin will differ depending on the framework involved.

Some frameworks offer built-in ways to visualize certain origins. For example, `ARView` and `ARSCNView` both have API to visualize the world origin for debugging:

```
view.debugOptions.insert(.showWorldOrigin)
```

`ARView` has additional API to visualize anchor origins:

```
view.debugOptions.insert(.showAnchorOrigins)
```

Other frameworks may not have origin visualization API to aid in debugging, but it is always possible to write visualization code for any coordinate space. For example, this snippet visualizes the origin of any SwiftUI `View`:

```
import SwiftUI

extension View {
    /// Visualizes the origin of any View for debugging purposes.
    /// The x-axis is red, the y-axis is green.
    public func showOrigin() -> some View {
        modifier(CoordinateAxes())
    }
}

private struct CoordinateAxes: ViewModifier {

    func body(content: Content) -> some View {
        content.overlay {

            GeometryReader { geometry in

                let size = geometry.size

                let smallestDim = min(size.width, size.height)

                // Set length to be at least 20 points.
                let length = max(smallestDim * 0.2, 20)
                let thickness = length / 7

                // X-axis.
                Color.red
                    .frame(width: length, height: thickness)
                    .position(.init(x: length / 2, y: thickness / 2))

                // Y-axis.
                Color.green
                    .frame(width: thickness, height: length)
                    .position(.init(x: thickness / 2, y: length / 2))
            }
        }
    }
}
```

Visualizing an origin could be all that is necessary to realize where the error is.

## Understand input expectations

Sometimes an API requires inputs that are already in a particular coordinate space. Otherwise its output is invalid.

Consider the `UIView` method, hitTest(_:with:). This method accepts a `CGPoint` as input, and uses it to perform a hit-test on the view. The problem here is that its results aren’t valid for *any* `CGPoint`, you must provide a `CGPoint` in the view’s local coordinate space to get a valid result.

When you have results that don’t make sense, it is a good idea to evaluate the APIs you are using to produce the results, and verify that you have provided inputs to them in the coordinate spaces they are expecting.

## Use known points

Using known points is an effective graphics debugging technique.

Consider an app that runs a `VNDetectRectanglesRequest` on a `CMSampleBuffer` stream, displays the stream in an `AVCaptureVideoPreviewLayer`, and then attempts to draw the detected rectangles on top of the preview layer in an overlay `CALayer`, but the drawing doesn’t appear as expected. After gaining an understanding of each coordinate space involved in the drawing process (the `AVCaptureVideoPreviewLayer`, the overlay `CALayer`, and the `VNRectangleObservation`) by visualizing their origins, it can be helpful to draw a known point, instead of trying to debug this on the fly with a dynamic video stream. In this specific example, you might use `CGRect(x: 0, y: 0, width: 0.25, height: 0.25)` as the input, a rectangle that you would expect to cover one quarter of the preview image when drawn correctly.

Being consistent with the data you feed through a coordinate conversion pipeline allows you to clearly see the effects of any changes you make when debugging.

## Log transforms and bounding boxes

Logging the transform and bounding box of a visual element is a simple but effective debugging technique.

Consider a scenario where your app is inserting a 3D model into a scene, but you don’t see the 3D model where you expected to see it. By logging the transform and bounding box of the model, you discover that the scale and the bounding box of the model is very large. This is a very good indication that the model is so large that the current viewpoint of the 3D scene is *inside* of the model. You remedy the situation by setting the model’s scale factor to a smaller value.

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

TN3158: Resolving Xcode 15 device connection issues

Identify software preventing Xcode 15 from connecting to Apple devices, and modify your configuration to allow these connections.

