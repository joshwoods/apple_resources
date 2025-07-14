

- MapKit
- MapKit for AppKit and UIKit
-  Displaying an Indoor Map 

Sample Code

# Displaying an Indoor Map

Use the Indoor Mapping Data Format (IMDF) to show an indoor map with custom overlays and points of interest.

Download

iOS 17.6+iPadOS 17.6+Xcode 16.0+

## Overview

The sample app demonstrates decoding, rendering, and styling of a small subset of the IMDF feature types and their properties. Use these examples to create your own indoor map with a style that’s consistent with your app’s design. You’ll need to handle feature categories that are specific to your venue, and configure the map style using your own colors, icons, and level picker.

Note

This sample code project is associated with WWDC 2019 session 241: Adding Indoor Maps to your App and Website.

## See Also

### Geographical features

class MKGeoJSONDecoder

An object that decodes GeoJSON objects into MapKit types.

class MKGeoJSONFeature

The decoded representation of a GeoJSON feature.

protocol MKGeoJSONObject

Objects that the GeoJSON decoder can return.

