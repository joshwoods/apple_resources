

- Core Location
- CLError
- CLError.Code
-  CLError.Code.regionMonitoringFailure 

Case

# CLError.Code.regionMonitoringFailure

A constant that indicates the location manager failed to monitor a registered region.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case regionMonitoringFailure
```

## Discussion

Monitoring can fail if the app exceeds the maximum number of regions that it can monitor simultaneously. Monitoring can also fail if the region’s radius distance is too large.

## See Also

### Getting region monitoring errors

case regionMonitoringDenied

A constant that indicates the user denied access to the region monitoring service.

case regionMonitoringSetupDelayed

A constant that indicates Core Location failed to initialize the region monitoring feature.

case regionMonitoringResponseDelayed

A constant that indicates Core Location will deliver events but they may be delayed.

