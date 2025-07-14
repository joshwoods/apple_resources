

- HomeKit
-  HMCameraView 

Class

# HMCameraView

The view into which a video stream or an image snapshot is rendered.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
class HMCameraView
```

## Topics

### Getting the Camera Source

var cameraSource: HMCameraSource?

class HMCameraSource

An abstract class for a camera’s data source.

### Initializers

init()

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

### Managing camera profiles

struct CameraView

A SwiftUI view into which a video stream or an image snapshot is rendered.

var cameraProfiles: [HMCameraProfile]?

An array of camera profiles implemented by the accessory.

class HMCameraProfile

A camera profile that interacts with an accessory’s camera.

