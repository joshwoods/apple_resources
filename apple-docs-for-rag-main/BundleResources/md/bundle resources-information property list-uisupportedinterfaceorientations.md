

- Bundle Resources
- Information Property List
-  UISupportedInterfaceOrientations 

Property List Key

# UISupportedInterfaceOrientations

The interface orientations supported by your app.

iOS 3.2+iPadOS 3.2+

## Details 

Name  
Supported interface orientations

Type  

array of strings

## Possible Values 

`UIInterfaceOrientationPortrait`  

The app supports the display in portrait mode, with the device upright and the front camera at the top.

`UIInterfaceOrientationPortraitUpsideDown`  

The app supports the display in portrait mode but is upside down, with the device upright and the front camera at the bottom. UIViewController ignores this option on devices without a Home button.

`UIInterfaceOrientationLandscapeLeft`  

The app supports the display in landscape mode, with the device upright and the front camera on the right.

`UIInterfaceOrientationLandscapeRight`  

The app supports the display in landscape mode, with the device upright and the front camera on the left.

## Attributes 

Default: `UIInterfaceOrientationPortrait`

## See Also

### Orientation

UIInterfaceOrientation

The initial orientation of the app’s user interface.

**Name:** Initial interface orientation

UIPreferredDefaultInterfaceOrientation

A string that indicates the preferred initial interface orientation for iPad and iPhone apps running on visionOS.

