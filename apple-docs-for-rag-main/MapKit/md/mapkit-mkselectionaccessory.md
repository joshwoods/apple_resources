

- MapKit
-  MKSelectionAccessory 

Class

# MKSelectionAccessory

The type of accessory to display for a selected annotation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
class MKSelectionAccessory
```

## Mentioned in 

Identifying unique locations with Place IDs

## Overview

Implement mapView(_:selectionAccessoryFor:) in your map view delegate to specify a selection accessory for annotation content.

## Topics

### Creating a selection accessory

class func mapItemDetail(MKSelectionAccessory.MapItemDetailPresentationStyle) -> MKSelectionAccessory

Detailed information about a place

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Place information

protocol MKMapItemDetailViewControllerDelegate

The methods that you use to receive events from an associated map view controller.

class MKMapItemDetailViewController

An object that displays detailed information about a map item.

class MapItemDetailPresentationStyle

The type of map item detail accessory presentation to use.

enum CalloutStyle

The style to use for a map item detail callout presentation.

