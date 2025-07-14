

- Core Location
- CLError
- CLError.Code
-  CLError.Code.regionMonitoringResponseDelayed 

Case

# CLError.Code.regionMonitoringResponseDelayed

A constant that indicates Core Location will deliver events but they may be delayed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case regionMonitoringResponseDelayed
```

## Discussion

The user information dictionary might contain an alternate region that you can monitor instead. Use kCLErrorUserInfoAlternateRegionKey to retrieve the CLRegion object.

## See Also

### Getting region monitoring errors

case regionMonitoringDenied

A constant that indicates the user denied access to the region monitoring service.

case regionMonitoringFailure

A constant that indicates the location manager failed to monitor a registered region.

case regionMonitoringSetupDelayed

A constant that indicates Core Location failed to initialize the region monitoring feature.

