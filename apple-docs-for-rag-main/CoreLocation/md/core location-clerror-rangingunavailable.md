

- Core Location
- CLError
-  rangingUnavailable 

Type Property

# rangingUnavailable

A constant that indicates ranging is disabled.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var rangingUnavailable: CLError.Code { get }
```

## Discussion

This error might occur if the device is in Airplane mode or if Bluetooth or location services are disabled.

## See Also

### Getting general errors

static var locationUnknown: CLError.Code

A constant that indicates the location manager was unable to obtain a location value right now.

static var denied: CLError.Code

A constant that indicates the user denied access to the location service.

static var promptDeclined: CLError.Code

A constant that indicates the user didn’t grant the requested temporary authorization.

static var network: CLError.Code

A constant that indicates the network was unavailable or a network error occurred.

static var headingFailure: CLError.Code

A constant that indicates the location manager can’t determine the heading.

static var rangingFailure: CLError.Code

A constant that indicates a general ranging error occurred.

enum Code

Error codes returned by the location manager object.

