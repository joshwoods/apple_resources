

- UIKit
- App and environment
-  Responding to changing display modes on Apple TV 

Article

# Responding to changing display modes on Apple TV

Change images and resources dynamically when the screen gamut on your device changes.

## Overview

On Apple TV (5th generation), the assets required for an app depend on the screen gamut of the TV being used, with 4K TVs using the Display P3 gamut, and all other resolutions using the sRGB gamut. Also, the screen gamut of the TV can change at any time, switching between 4K and other resolutions. Your app needs to respond to these changes and present the appropriate assets when required.

### Create and place the image assets

In Xcode, create an image asset in an asset catalog. In the Attributes inspector, configure the asset catalog to handle Display P3 images. In the Devices pane, ensure that Apple TV is selected. From the Gamut menu, select sRGB and Display P3. The following image shows the correct settings.

### Add images to the asset catalog

Place non-4K images in the 1x (sRGB) slot and 4K images in the 2x (Display P3) slot. The correct image is automatically loaded based on the display gamut of the TV. The following image shows assets placed in their correct containers.

### Adapt to screen changes programmatically

Implement the traitCollectionDidChange(_:) method to respond to changing device traits. If your app performs expensive operations related to image generation based on the current display gamut, it’s important to verify that the display gamut has changed before performing these operations. The following code shows how to test whether the display gamut changed.

```
override func traitCollectionDidChange(_ previousTraitCollection: UITraitCollection?) {
    let currentDisplayGamut = self.traitCollection.displayGamut
    if (previousTraitCollection?.displayGamut == .SRGB) && (currentDisplayGamut == .SRGB) {
        // Resolution didn't change. Your code goes here.
    } else if (previousTraitCollection?.displayGamut == .P3) && (currentDisplayGamut == .P3) {
        // Resolution didn't change. Your code goes here.
    } else {
        // Resolution changed. Your code goes here.
    }
}
```

## See Also

### Adaptivity

Automatic trait tracking

Reduce the need to manually register for trait changes when you use traits within a method or closure that supports automatic trait tracking.

class UITraitCollection

A collection of data that represents the environment for an individual element in your app’s user interface.

protocol UITraitEnvironment

A set of methods that makes the iOS interface environment available to your app.

protocol UITraitChangeObservable

A type that calls your code in reaction to changes in the trait environment.

protocol UIMutableTraits

A mutable container of traits.

protocol UIAdaptivePresentationControllerDelegate

A set of methods that, in conjunction with a presentation controller, determine how to respond to trait changes in your app.

protocol UIContentContainer

A set of methods for adapting the contents of your view controllers to size and trait changes.

