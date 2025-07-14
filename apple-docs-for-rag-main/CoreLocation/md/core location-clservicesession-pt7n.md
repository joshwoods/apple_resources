

- Core Location
-  CLServiceSession 

Class

# CLServiceSession

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
final class CLServiceSession
```

## Mentioned in 

Handling location updates in the background

Configuring your app to use location services

Suspending authorization requests

## Topics

### Classes

class Diagnostics

### Structures

struct Diagnostic

### Initializers

init(authorization: CLServiceSession.AuthorizationRequirement)

init(authorization: CLServiceSession.AuthorizationRequirement, fullAccuracyPurposeKey: String)

### Instance Properties

var diagnostics: CLServiceSession.Diagnostics

### Instance Methods

func invalidate()

### Enumerations

enum AuthorizationRequirement

## Relationships

### Conforms To

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

struct CLLocationCoordinate2D

The latitude and longitude associated with a location, specified using the WGS 84 reference frame.

class CLFloor

The floor of a building on which the user’s device is located.

class CLVisit

Information about the user’s location during a specific period of time.

class CLLocationSourceInformation

Information about the source that provides a location.

Monitoring location changes with Core Location

Define boundaries and act on user location updates.

