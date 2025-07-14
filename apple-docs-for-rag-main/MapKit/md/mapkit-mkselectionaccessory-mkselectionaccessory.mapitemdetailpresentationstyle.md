

- MapKit
- MKSelectionAccessory
-  MKSelectionAccessory.MapItemDetailPresentationStyle 

Class

# MKSelectionAccessory.MapItemDetailPresentationStyle

The type of map item detail accessory presentation to use.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
class MapItemDetailPresentationStyle
```

## Topics

### Creating a presentation style

static func automatic(presentationViewController: UIViewController?) -> MKSelectionAccessory.MapItemDetailPresentationStyle

An appropriate presentation style will be chosen automatically.

static func automatic(presentationViewController: NSViewController?) -> MKSelectionAccessory.MapItemDetailPresentationStyle

An appropriate presentation style will be chosen automatically.

class var callout: MKSelectionAccessory.MapItemDetailPresentationStyle

Show map item detail as an annotation callout on the map.

static func callout(MKSelectionAccessory.MapItemDetailPresentationStyle.CalloutStyle) -> MKSelectionAccessory.MapItemDetailPresentationStyle

Show map item detail as an annotation callout on the map

class var openInMaps: MKSelectionAccessory.MapItemDetailPresentationStyle

Display a small “Open in Apple Maps” link.

class func sheet(presentedFrom: UIViewController) -> MKSelectionAccessory.MapItemDetailPresentationStyle

Show map item detail by presenting a sheet.

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

class MKSelectionAccessory

The type of accessory to display for a selected annotation.

enum CalloutStyle

The style to use for a map item detail callout presentation.

