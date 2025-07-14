

- Core Location
- CLLocationManager
-  monitoredRegions 

Instance Property

# monitoredRegions

The set of shared regions monitored by all location-manager objects.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+

``` source
var monitoredRegions: Set { get }
```

## Discussion

You cannot add regions to this property directly. Instead, you must register regions by calling the startMonitoring(for:) method. The regions in this property are shared by all instances of the CLLocationManager class in your app.

The objects in this set may not necessarily be the same objects you specified at registration time. Only the region data itself is maintained by the system. Therefore, the only way to uniquely identify a registered region is using its identifier property.

The location manager persists region data between launches of your app. If your app is terminated and then relaunched, the contents of this property are repopulated with region objects that contain the previously registered data.

In a compatible iPad or iPhone app running in visionOS, the property contains an empty set.

## See Also

### Running the region-monitoring service

var maximumRegionMonitoringDistance: CLLocationDistance

The largest boundary distance that can be assigned to a region.

