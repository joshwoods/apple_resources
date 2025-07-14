

- Bundle Resources
- Information Property List
-  UIInterfaceOrientation 

Property List Key

# UIInterfaceOrientation

The initial orientation of the app’s user interface.

iOS 2.0+iPadOS 2.0+

## Details 

Name  
Initial interface orientation

Type  

string

## Possible Values 

`UIInterfaceOrientationPortrait`  

The device is in portrait mode, with the device upright and the Home button on the bottom.

`UIInterfaceOrientationPortraitUpsideDown`  

The device is in portrait mode but is upside down, with the device upright and the Home button at the top.

`UIInterfaceOrientationLandscapeLeft`  

The device is in landscape mode, with the device upright and the Home button on the left.

`UIInterfaceOrientationLandscapeRight`  

The device is in landscape mode, with the device upright and the Home button on the right.

## Attributes 

Default: `UIInterfaceOrientationPortrait`

## Discussion

The default value is `UIInterfaceOrientationPortrait`. If you add the UISupportedInterfaceOrientations key to the information property list, the system ignores this key.

For more information, see UIInterfaceOrientation.

## See Also

### Orientation

UISupportedInterfaceOrientations

The interface orientations supported by your app.

**Name:** Supported interface orientations

UIPreferredDefaultInterfaceOrientation

A string that indicates the preferred initial interface orientation for iPad and iPhone apps running on visionOS.

