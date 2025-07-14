

- MapKit
- MKPlacemark
-  init(coordinate:) 

Initializer

# init(coordinate:)

Creates and returns a placemark object using the specified coordinate.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(coordinate: CLLocationCoordinate2D)
```

## Parameters 

`coordinate`  

The geographic coordinate to associate with the placemark.

## Return Value

An initialized MKPlacemark object.

## Discussion

This method doesn’t fill in any of the other inherited properties describing the location.

## See Also

### Creating a placemark object

init(coordinate: CLLocationCoordinate2D, postalAddress: CNPostalAddress)

Creates and returns a placemark object with the specified coordinate and postal address from the user’s Contacts database.

init(coordinate: CLLocationCoordinate2D, addressDictionary: [String : Any]?)

Creates and returns a placemark object using the specified coordinate and Address Book dictionary.

