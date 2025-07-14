

- MapKit
-  MKMapItemDetailViewControllerDelegate 

Protocol

# MKMapItemDetailViewControllerDelegate

The methods that you use to receive events from an associated map view controller.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
protocol MKMapItemDetailViewControllerDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func mapItemDetailViewControllerDidFinish(MKMapItemDetailViewController)

Informs the delegate when a person dismissed the view controller.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Place information

class MKMapItemDetailViewController

An object that displays detailed information about a map item.

class MapItemDetailPresentationStyle

The type of map item detail accessory presentation to use.

class MKSelectionAccessory

The type of accessory to display for a selected annotation.

enum CalloutStyle

The style to use for a map item detail callout presentation.

