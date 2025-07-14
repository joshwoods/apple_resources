

- Image I/O
-  GPS Dictionary Keys 

API Collection

# GPS Dictionary Keys

Keys for Global Positioning System (GPS) information.

## Topics

### Dictionary

let kCGImagePropertyGPSDictionary: CFString

A dictionary of key-value pairs for an image that has Global Positioning System (GPS) information.

### GPS Coordinate

let kCGImagePropertyGPSLatitude: CFString

The latitude.

let kCGImagePropertyGPSLongitude: CFString

The longitude.

let kCGImagePropertyGPSAltitude: CFString

The altitude.

let kCGImagePropertyGPSLatitudeRef: CFString

An indication of whether the latitude is north or south.

let kCGImagePropertyGPSLongitudeRef: CFString

An indication of whether the longitude is east or west.

let kCGImagePropertyGPSAltitudeRef: CFString

The altitude point of reference.

let kCGImagePropertyGPSHPositioningError: CFString

The horizontal error in the GPS position.

### Destinations

let kCGImagePropertyGPSDestLatitude: CFString

The latitude of the destination point.

let kCGImagePropertyGPSDestLongitude: CFString

The longitude of the destination point.

let kCGImagePropertyGPSDestBearing: CFString

The bearing to the destination point.

let kCGImagePropertyGPSDestDistance: CFString

The distance to the destination point.

let kCGImagePropertyGPSDestLatitudeRef: CFString

An indication of whether the latitude of the destination point is northern or southern.

let kCGImagePropertyGPSDestLongitudeRef: CFString

An indication of whether the longitude of the destination point is east or west.

let kCGImagePropertyGPSDestBearingRef: CFString

The reference for giving the bearing to the destination point.

let kCGImagePropertyGPSDestDistanceRef: CFString

The units for expressing the distance to the destination point.

### Image Orientation

let kCGImagePropertyGPSImgDirectionRef: CFString

The reference for the direction of the image.

let kCGImagePropertyGPSImgDirection: CFString

The direction of the image.

### Measurement Details

let kCGImagePropertyGPSStatus: CFString

The status of the GPS receiver.

let kCGImagePropertyGPSSatellites: CFString

The satellites used for GPS measurements.

let kCGImagePropertyGPSMeasureMode: CFString

The measurement mode.

let kCGImagePropertyGPSDOP: CFString

The degree of precision (DOP) of the data.

let kCGImagePropertyGPSSpeedRef: CFString

The unit for expressing the GPS receiver’s speed of movement.

let kCGImagePropertyGPSSpeed: CFString

The GPS receiver’s speed of movement.

let kCGImagePropertyGPSTrackRef: CFString

The reference for the direction of GPS receiver’s movement.

let kCGImagePropertyGPSTrack: CFString

The direction of GPS receiver’s movement.

let kCGImagePropertyGPSMapDatum: CFString

The geodetic survey data used by the GPS receiver.

let kCGImagePropertyGPSProcessingMethod: CFString

The name of the method used to find a location.

let kCGImagePropertyGPSAreaInformation: CFString

The name of the GPS area.

let kCGImagePropertyGPSDifferental: CFString

An indication of whether differential correction is applied to the GPS receiver.

### Timestamp Information

let kCGImagePropertyGPSTimeStamp: CFString

The time in UTC (Coordinated Universal Time).

let kCGImagePropertyGPSDateStamp: CFString

The date and time information relative to Coordinated Universal Time (UTC).

### GPS Version

let kCGImagePropertyGPSVersion: CFString

The GPS version information.

## See Also

### Common Image Properties

Image Properties

Properties that apply to the container in general, and not necessarily to an individual image in the container.

EXIF Dictionary Keys

Metadata keys for Exchangeable Image File Format (EXIF) data.

IPTC Dictionary Keys

Metadata keys for International Press Telecommunications Council (IPTC) data.

WebP Data

Metadata keys for WebP metadata.

