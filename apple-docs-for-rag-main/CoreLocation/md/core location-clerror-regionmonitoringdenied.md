

- Core Location
- CLError
-  regionMonitoringDenied 

Type Property

# regionMonitoringDenied

A constant that indicates the user denied access to the region monitoring service.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var regionMonitoringDenied: CLError.Code { get }
```

## See Also

### Getting region monitoring errors

static var regionMonitoringFailure: CLError.Code

A constant that indicates the location manager failed to monitor a registered region.

static var regionMonitoringSetupDelayed: CLError.Code

A constant that indicates Core Location couldn’t initialize the region monitoring feature immediately.

static var regionMonitoringResponseDelayed: CLError.Code

A constant that indicates Core Location will deliver events but they may be delayed.

