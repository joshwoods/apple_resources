

- MapKit
- MKMapSnapshotter
-  MKMapSnapshotter.Options 

Class

# MKMapSnapshotter.Options

The options the snapshotter initializer uses to create a snapshotter to capture map-based imagery.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
class Options
```

## Overview

After creating and configuring an instance of this class, you pass that instance to an MKMapSnapshotter object. The snapshotter uses the configuration options to determine which portion of the map to capture, the viewing angle to use for the camera, and the map’s overall appearance.

In macOS 10.14 and later, you can apply a light or dark appearance to your map snapshots by modifying the appearance property of your snapshot options. Even if you specify a custom appearance, users can use the Maps app to force all maps to adopt a light appearance.

## Topics

### Configuring the snapshot region

var region: MKCoordinateRegion

The area of the map that you want to capture.

var mapRect: MKMapRect

The map rectangle that you want to capture.

var camera: MKMapCamera

The camera to use when taking the map snapshot.

### Configuring the map data

var preferredConfiguration: MKMapConfiguration

The map configuration style to use for snapshots.

var mapType: MKMapType

The map’s visual style.

Deprecated

var showsBuildings: Bool

A Boolean that indicates whether the map displays extruded building information.

Deprecated

var pointOfInterestFilter: MKPointOfInterestFilter?

The filter to use for determining the points of interest that appear in the snapshot.

Deprecated

var showsPointsOfInterest: Bool

A Boolean value that indicates whether the map displays point-of-interest information.

Deprecated

### Configuring the image output

var traitCollection: UITraitCollection

Traits that determine the appearance of the map snapshot.

var size: CGSize

The size of the image that you want to create.

var appearance: NSAppearance?

The visual style (light or dark) to apply to the map when rendering the snapshot image.

var scale: CGFloat

The scale factor to use when creating the image.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating a snapshotter object

init(options: MKMapSnapshotter.Options)

Creates and returns a snapshotter object based on the specified options.

