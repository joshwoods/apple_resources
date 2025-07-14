

- Core Location
- CLError
-  regionMonitoringFailure 

Type Property

# regionMonitoringFailure

A constant that indicates the location manager failed to monitor a registered region.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var regionMonitoringFailure: CLError.Code { get }
```

## Discussion

Monitoring can fail if the app exceeds the maximum number of regions that it can monitor simultaneously. Monitoring can also fail if the region’s radius distance is too large.

## See Also

### Getting region monitoring errors

static var regionMonitoringDenied: CLError.Code

A constant that indicates the user denied access to the region monitoring service.

static var regionMonitoringSetupDelayed: CLError.Code

A constant that indicates Core Location couldn’t initialize the region monitoring feature immediately.

static var regionMonitoringResponseDelayed: CLError.Code

A constant that indicates Core Location will deliver events but they may be delayed.

