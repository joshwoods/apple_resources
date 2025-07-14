

- MapKit
-  MKMapPoint 

Structure

# MKMapPoint

A point on a two-dimensional map projection.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MKMapPoint
```

## Overview

If you project the curved surface of the globe onto a flat surface, you get a two-dimensional version of a map where longitude lines appear to be parallel. An `MKMapPoint` data structure represents a point on this two-dimensional map.

The underlying units that MapKit uses to draw the contents of an MKMapView define the actual units of a map point, but you don’t need to worry about these units directly. You use map points primarily to simplify computations that are complex to do using coordinate values on a curved surface. By converting to map points, you can perform those calculations on a flat surface, which is generally much simpler, and then convert back as necessary. You can map between coordinate values and map points using the init(_:) and coordinate functions.

When saving map-related data to a file, save coordinate values (latitude and longitude) rather than map points.

## Topics

### Creating a map point

init()

Creates a map point at an unspecified point.

init(x: Double, y: Double)

Creates a new map point structure from the specified values.

init(CLLocationCoordinate2D)

Creates the map point data structure that corresponds to the specified coordinate.

### Getting the point coordinates

var x: Double

The location of the point along the x-axis of the map.

var y: Double

The location of the point along the y-axis of the map.

var coordinate: CLLocationCoordinate2D

A 2D coordinate that corresponds to the latitude and longitude of the specified map point.

### Comparing map points

func MKMapPointEqualToPoint(MKMapPoint, MKMapPoint) -> Bool

Returns a Boolean value that indicates whether two map points are equal.

### Getting the distance between points

func distance(to: MKMapPoint) -> CLLocationDistance

Returns the number of meters between two map points.

func MKMetersPerMapPointAtLatitude(CLLocationDegrees) -> CLLocationDistance

Returns the distance that one map point spans at the specified latitude.

func MKMapPointsPerMeterAtLatitude(CLLocationDegrees) -> Double

Returns the number of map points that represent one meter at the specified latitude.

### Getting a description of the point

func MKStringFromMapPoint(MKMapPoint) -> String

Returns a formatted string for the specified map point.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Map coordinates

struct MKCoordinateRegion

A rectangular geographic region that centers around a specific latitude and longitude.

struct MKCoordinateSpan

The width and height of a map region.

struct MKMapRect

A rectangular area on a two-dimensional map projection.

struct MKMapSize

Width and height information on a two-dimensional map projection.

class MKDistanceFormatter

A utility object that converts between a geographic distance and a string-based expression of that distance.

