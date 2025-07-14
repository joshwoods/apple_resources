

- CarPlay
-  CPPointOfInterest 

Class

# CPPointOfInterest

An object that describes a point of interest on the template’s map and in its scrollable picker.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPPointOfInterest
```

## Overview

A point of interest describes a geographical location on a map. It also provides supplementary information about the location, such as a title and summary that the template displays in a scrollable picker and on a detail card. A point of interest also provides the buttons the detail card presents to the user as contextual actions.

You provide an array of `CPPointOfInterest` objects when initializing CPPointOfInterestTemplate, or whenever the visible region of the template’s map changes, by calling the template’s setPointsOfInterest(_:selectedIndex:) method.

`CPPointOfInterestTemplate` displays a maximum of twelve points of interest.

## Topics

### Creating a Point of Interest

convenience init(location: MKMapItem, title: String, subtitle: String?, summary: String?, detailTitle: String?, detailSubtitle: String?, detailSummary: String?, pinImage: UIImage?)

Creates a point of interest for a specific location.

### Managing the Map Annotation

var location: MKMapItem

The map item that contains the point of interest’s geographical information.

var pinImage: UIImage?

A custom image that the map annotation displays.

### Managing the Picker Item’s Data

var title: String

The title that the picker’s item displays.

var subtitle: String?

The subtitle that the picker’s item displays.

var summary: String?

The summary that the picker’s item displays.

### Managing the Detail Card’s Data

var detailTitle: String?

The detail card’s title.

var detailSubtitle: String?

The detail card’s subtitle.

var detailSummary: String?

The detail card’s summary.

### Managing the Detail Card’s Buttons

var primaryButton: CPTextButton?

The detail card’s primary action button.

var secondaryButton: CPTextButton?

The detail card’s secondary action button.

### Attaching Additional Context

var userInfo: Any?

An opaque value for the point of interest.

### Initializers

init(location: MKMapItem, title: String, subtitle: String?, summary: String?, detailTitle: String?, detailSubtitle: String?, detailSummary: String?, pinImage: UIImage?, selectedPinImage: UIImage?)

### Instance Properties

var selectedPinImage: UIImage?

### Type Properties

class var pinImageSize: CGSize

class var selectedPinImageSize: CGSize

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Creating a Point of Interest Template

init(title: String, pointsOfInterest: [CPPointOfInterest], selectedIndex: Int)

Creates a Point of Interest template with a title, the points of interest to display, and the initial selection’s index.

