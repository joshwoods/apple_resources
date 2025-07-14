

- MapKit
-  MKCoordinateSpan 

Structure

# MKCoordinateSpan

The width and height of a map region.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MKCoordinateSpan
```

## Overview

You use the delta values in this structure to indicate the desired zoom level of the map, with smaller delta values corresponding to a higher zoom level.

## Topics

### Creating a coordinate span

init()

Creates a coordinate span that represents a width and height on a map.

init(latitudeDelta: CLLocationDegrees, longitudeDelta: CLLocationDegrees)

Creates a new MKCoordinateSpan from the specified values.

### Getting the span coordinates

var latitudeDelta: CLLocationDegrees

The amount of north-to-south distance (measured in degrees) to display on the map.

var longitudeDelta: CLLocationDegrees

The amount of east-to-west distance (measured in degrees) to display for the map region.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable

## See Also

### Map coordinates

struct MKCoordinateRegion

A rectangular geographic region that centers around a specific latitude and longitude.

struct MKMapRect

A rectangular area on a two-dimensional map projection.

struct MKMapPoint

A point on a two-dimensional map projection.

struct MKMapSize

Width and height information on a two-dimensional map projection.

class MKDistanceFormatter

A utility object that converts between a geographic distance and a string-based expression of that distance.

