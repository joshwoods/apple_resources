

- Core Location
- CLLocationManagerDelegate
-  locationManager(\_:didUpdateLocations:) 

Instance Method

# locationManager(\_:didUpdateLocations:)

Tells the delegate that new location data is available.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func locationManager(
    _ manager: CLLocationManager,
    didUpdateLocations locations: [CLLocation]
)
```

## Parameters 

`manager`  

The location manager object that generated the update event.

`locations`  

An array of CLLocation objects containing the location data. This array always contains at least one object representing the current location. If updates were deferred or if multiple locations arrived before they could be delivered, the array may contain additional entries. The objects in the array are organized in the order in which they occurred. Therefore, the most recent location update is at the end of the array.

## Mentioned in 

Creating a location push service extension

## Discussion

Implementation of this method is optional but recommended.

## Topics

### Related Documentation

MapKit

Display map or satellite imagery within your app, call out points of interest, and determine placemark information for map coordinates.

MapKit JS

Embed interactive Apple Maps on your website, annotate points of interest, and perform georelated searches.

## See Also

### Receiving location updates

func locationManager(CLLocationManager, didUpdateTo: CLLocation, from: CLLocation)

Tells the delegate that a new location value is available.

Deprecated

func locationManager(CLLocationManager, didFinishDeferredUpdatesWithError: (any Error)?)

Tells the delegate that updates will no longer be deferred.

