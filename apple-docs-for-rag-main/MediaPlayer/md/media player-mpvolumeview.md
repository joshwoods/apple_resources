

- Media Player
-  MPVolumeView 

Class

# MPVolumeView

A slider control for setting the system audio output volume, and a button for choosing the audio output route.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class MPVolumeView
```

## Overview

Use a volume view to present the user with a slider control for setting the system audio output volume, and a button for choosing the audio output route when the option is available. When first displayed, the slider’s position reflects the current system audio output volume. As the user drags the slider, the changes update the volume view. If the user presses the device volume buttons while sound is playing, the slider moves to reflect the new volume.

If there’s an Apple TV or other AirPlay-enabled device in range, the route button allows the user to choose it. If there’s only one audio output route available, the view doesn’t display the route button. The view also doesn’t display a route button when the app runs in visionOS.

Important

You can’t change the volume or choose a route with this class while testing in the Simulator. These abilities only work on a device.

Use this class by embedding an instance of it in your view hierarchy. The following code snippet assumes you’ve placed an instance of the UIView class on a view using Interface Builder, sizing and positioning it as desired to contain the volume view. Point to the UIView instance with an outlet variable—named, in the case of this example, `mpVolumeViewParentView`. You’d typically place code like that shown in the following code in your `viewDidLoad` method.

Listing 1. Adding a volume view to your view hierarchy

```
parentView.backgroundColor = .clear
let volumeView = MPVolumeView(frame: parentView.bounds)
parentView.addSubview(volumeView)
```

When an audio output route that doesn’t support volume control, such as a car head unit, is active, the system replaces the volume slider with the route name.

To instead display a volume slider as an alert, use the functions described in Global volume setting methods.

Note

You can’t subclass the MPVolumeView class.

### Customizing the volume slider’s appearance

The volume slider is a UISlider object. Sliders are always displayed as horizontal bars and an indicator, or **thumb**, notes the current value of the slider, which the user can move to change the setting.

Slider controls draw the volume slider track using two distinct images, which are customizable. The system draws the region between the thumb and the end of the track associated with the slider’s minimum value using the **minimum volume slider image**. The system region between the thumb and the end of the track associated with the slider’s maximum value using the **maximum volume slider image**. You can assign different images to customize the appearance of the slider for its various states, such as enabled, disabled, and highlighted.

You can also customize the volume thumb image for the slider.

Note

The volume slider control provides a set of default images for both the track and thumb. The system uses the default images if you don’t specify any custom images.

## Topics

### Managing visibility of controls

var showsVolumeSlider: Bool

A Boolean value that indicates the volume slider is visible in the volume view.

### Customizing the volume slider

func maximumVolumeSliderImage(for: UIControl.State) -> UIImage?

Returns the maximum volume image associated with the specified control state.

func minimumVolumeSliderImage(for: UIControl.State) -> UIImage?

Returns the minimum volume image associated with the specified control state.

func setMaximumVolumeSliderImage(UIImage?, for: UIControl.State)

Assigns a maximum volume slider image to the specified control states.

func setMinimumVolumeSliderImage(UIImage?, for: UIControl.State)

Assigns a minimum volume slider image to the specified control states.

func setVolumeThumbImage(UIImage?, for: UIControl.State)

Assigns a thumb image to the specified control states.

func volumeSliderRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the slider’s track.

func volumeThumbImage(for: UIControl.State) -> UIImage?

Returns the thumb image associated with the specified control state.

func volumeThumbRect(forBounds: CGRect, volumeSliderRect: CGRect, value: Float) -> CGRect

Returns the drawing rectangle for the volume slider’s thumb image.

### Deprecated

var volumeWarningSliderImage: UIImage?

The image used to designate the European Union volume limit.

Deprecated

var showsRouteButton: Bool

A Boolean value that indicates whether the route button is visible in the volume view.

Deprecated

var areWirelessRoutesAvailable: Bool

A Boolean value indicating wireless routes are available.

Deprecated

var isWirelessRouteActive: Bool

A Boolean value that indicates whether the wireless route is active.

Deprecated

func routeButtonImage(for: UIControl.State) -> UIImage?

Returns the button image associated with the specified control state.

Deprecated

func routeButtonRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the route button.

Deprecated

func setRouteButtonImage(UIImage?, for: UIControl.State)

Assigns a button image to the specified control states.

Deprecated

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Media player user interface

Displaying a media picker from your app

Let users choose the music they want to play by displaying a media picker interface from within your app.

class MPMediaPickerController

A specialized view controller that provides a graphical interface for selecting media items.

