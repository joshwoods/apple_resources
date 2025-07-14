

- Core Location
-  CLLocationCoordinate2D 

Structure

# CLLocationCoordinate2D

The latitude and longitude associated with a location, specified using the WGS 84 reference frame.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct CLLocationCoordinate2D
```

## Topics

### Creating a location coordinate

init()

Creates a location coordinate object.

init(latitude: CLLocationDegrees, longitude: CLLocationDegrees)

Creates a location coordination object with the specified latitude and longitude values.

func CLLocationCoordinate2DMake(CLLocationDegrees, CLLocationDegrees) -> CLLocationCoordinate2D

Formats a latitude and longitude value into a coordinate data structure format.

### Getting the geographic coordinates

var latitude: CLLocationDegrees

The latitude in degrees.

var longitude: CLLocationDegrees

The longitude in degrees.

### Validating a coordinate

func CLLocationCoordinate2DIsValid(CLLocationCoordinate2D) -> Bool

Returns a Boolean value indicating whether the specified coordinate is valid.

let kCLLocationCoordinate2DInvalid: CLLocationCoordinate2D

An invalid coordinate value.

## Relationships

### Conforms To

- Animatable
- BitwiseCopyable
- Copyable
- Decodable
- Encodable
- Sendable

## See Also

### Location updates

Getting the current location of a device

Start location services and provide information the system needs to optimize power usage for those services.

Handling location updates in the background

Configure your app to receive location updates when it isn’t running in the foreground.

Creating a location push service extension

Add and configure an extension to enable your location-sharing app to access a user’s location in response to a request from another user.

class CLLocation

The latitude, longitude, and course information reported by the system.

class CLFloor

The floor of a building on which the user’s device is located.

class CLVisit

Information about the user’s location during a specific period of time.

class CLLocationSourceInformation

Information about the source that provides a location.

Monitoring location changes with Core Location

Define boundaries and act on user location updates.

class CLServiceSession

