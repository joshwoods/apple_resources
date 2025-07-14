

- Core Location
- CLLocationManager
-  maximumRegionMonitoringDistance 

Instance Property

# maximumRegionMonitoringDistance

The largest boundary distance that can be assigned to a region.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+

``` source
var maximumRegionMonitoringDistance: CLLocationDistance { get }
```

## Discussion

This property defines the largest boundary distance allowed from a region’s center point. Attempting to monitor a region with a distance larger than this value causes the location manager to send a CLError.Code.regionMonitoringFailure error to the delegate.

If region monitoring is unavailable or not supported, the value in this property is `-1`.

## See Also

### Running the region-monitoring service

var monitoredRegions: Set&lt;CLRegion>

The set of shared regions monitored by all location-manager objects.

