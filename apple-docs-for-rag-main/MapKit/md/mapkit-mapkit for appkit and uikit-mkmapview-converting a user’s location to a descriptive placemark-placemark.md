

- MapKit
- MapKit for AppKit and UIKit
- MKMapView
-  Converting a user’s location to a descriptive placemark 

Article

# Converting a user’s location to a descriptive placemark

Transform the user’s location that displays on a map into an informative textual description by reverse geocoding.

## Overview

You can show a user’s location on a map in order to orient them to elements of your app that use map content. For instance, a user’s current location can be a point of reference for retrieving search results or calculating directions. Additionally, you can display location information outside of the map, such as a search field pre-filled with the user’s current city or street address. To provide this information in your app, configure your map view to display the user’s location, and then translate the location to informative, user-friendly data.

### Display the user location annotation

To provide user-friendly place information, configure your map view to display the user’s current location by enabling showsUserLocation. After enabling this property, the map delegate begins receiving updates to the user’s location, represented with a MKUserLocation object, through mapView(_:didUpdate:).

### Geocode the user location annotation

CLPlacemark objects represent user place names, and include properties for street name, city name, country or region name, and many other location identifiers. When mapView(_:didUpdate:) receives updates on the user’s location, convert the MKUserLocation object to a CLPlacemark by reverse geocoding the location property with a CLGeocoder. Readable descriptions of the user’s location are available as properties on the placemark, such as the city information stored in the locality property.

Important

Geocoding requests are rate-limited for each app. Issue new geocoding requests only when the user has moved a significant distance and after a reasonable amount of time has passed.

```
func mapView(_ mapView: MKMapView, didUpdate userLocation: MKUserLocation) {
        guard let newLocation = userLocation.location else { return }

        let currentTime = Date()
        let lastLocation = self.currentLocation
        self.currentLocation = newLocation

        // Only get new placemark information if you don't have a previous location,
        // if the user has moved a meaningful distance from the previous location, such as 1000 meters,
        // and if it's been 60 seconds since the last geocode request.
        if let lastLocation = lastLocation,
            newLocation.distance(from: lastLocation) 

## See Also

### Related Documentation

Converting between coordinates and user-friendly place names

Convert between a latitude and longitude pair and a more user-friendly description of that location.

### Displaying the user’s location

var showsUserLocation: Bool

A Boolean value that indicates whether the map tries to display the user’s location.

var isUserLocationVisible: Bool

A Boolean value that indicates whether the user’s location is visible in the map view.

var userLocation: MKUserLocation

The annotation object that represents the user’s location.

var userTrackingMode: MKUserTrackingMode

The mode to use for tracking the user’s location.

func setUserTrackingMode(MKUserTrackingMode, animated: Bool)

Sets the mode to use for tracking the user’s location, with optional animation.

enum MKUserTrackingMode

The mode to use for tracking the user’s location on the map.

