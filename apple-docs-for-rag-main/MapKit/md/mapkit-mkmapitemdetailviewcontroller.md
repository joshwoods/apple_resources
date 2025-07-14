

- MapKit
-  MKMapItemDetailViewController 

Class

# MKMapItemDetailViewController

An object that displays detailed information about a map item.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
class MKMapItemDetailViewController
```

## Overview

The view controller presents modally and displays place information such as addresses and phone numbers.

This class doesn’t support subclassing. The view hierarchy for this class is private and must not be modified.

## Topics

### Creating a map item detail view controller

init(mapItem: MKMapItem?)

Create a map item detail view controller.

init(mapItem: MKMapItem?, displaysMap: Bool)

Create a map item detail view controller

### Dismissing the map item detail interface

var delegate: (any MKMapItemDetailViewControllerDelegate)?

The map item detail view controller’s delegate.

### Getting and setting the map item

var mapItem: MKMapItem?

The map item to display.

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

### Place information

protocol MKMapItemDetailViewControllerDelegate

The methods that you use to receive events from an associated map view controller.

class MapItemDetailPresentationStyle

The type of map item detail accessory presentation to use.

class MKSelectionAccessory

The type of accessory to display for a selected annotation.

enum CalloutStyle

The style to use for a map item detail callout presentation.

