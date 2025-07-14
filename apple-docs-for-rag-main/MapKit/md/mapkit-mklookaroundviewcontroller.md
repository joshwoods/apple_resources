

- MapKit
-  MKLookAroundViewController 

Class

# MKLookAroundViewController

A class that manages the presentation and display of a LookAround view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@MainActor
class MKLookAroundViewController
```

## Topics

### Creating a LookAround controller

init?(coder: NSCoder)

Creates a new LookAround view controller object from a coder object provided by a storyboard or nib file.

init(nibName: String?, bundle: Bundle?)

Creates a new LookAround view controller from the specified nib and bundle.

init(scene: MKLookAroundScene)

Creates a new LookAround view controller with the specified scene.

### Customizing the LookAround display

var isNavigationEnabled: Bool

A Boolean value that indicates whether the map’s navigation controls are visible.

var pointOfInterestFilter: MKPointOfInterestFilter?

The filter used to determine the points of interest shown on the map.

var showsRoadLabels: Bool

A Boolean value that indicates whether the map display road labels.

var badgePosition: MKLookAroundBadgePosition

A value that indicates the badge’s position on the LookAround view.

enum MKLookAroundBadgePosition

Constants that control the position of badges on LookAround views.

### Interacting with the controller

var delegate: (any MKLookAroundViewControllerDelegate)?

An object you provide to receive events related to the user’s interaction with the LookAround view controller.

protocol MKLookAroundViewControllerDelegate

Methods you implement to respond to changes in the LookAround view controller.

### Accessing the scene

var scene: MKLookAroundScene?

The LookAround scene.

## Relationships

### Inherits From

- NSViewController
- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSecureCoding
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Exploring at street level

class MKLookAroundScene

A utility class that encapsulates information the framework requires to retrieve and display a specific Look Around location’s imagery.

class MKLookAroundSceneRequest

A class you use to request a LookAround scene at the location you specify.

class MKLookAroundSnapshotter

A utility class that you use to create a static image from a LookAround scene.

