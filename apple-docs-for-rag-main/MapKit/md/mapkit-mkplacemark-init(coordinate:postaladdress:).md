

- MapKit
- MKPlacemark
-  init(coordinate:postalAddress:) 

Initializer

# init(coordinate:postalAddress:)

Creates and returns a placemark object with the specified coordinate and postal address from the user’s Contacts database.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
init(
    coordinate: CLLocationCoordinate2D,
    postalAddress: CNPostalAddress
)
```

## Parameters 

`coordinate`  

The geographic coordinate to associate with the placemark.

`postalAddress`  

An object containing the address information from the Contacts framework.

## Return Value

An initialized MKPlacemark object.

## See Also

### Creating a placemark object

init(coordinate: CLLocationCoordinate2D)

Creates and returns a placemark object using the specified coordinate.

init(coordinate: CLLocationCoordinate2D, addressDictionary: [String : Any]?)

Creates and returns a placemark object using the specified coordinate and Address Book dictionary.

