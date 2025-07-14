

- MapKit
- MKPlacemark
-  init(coordinate:addressDictionary:) 

Initializer

# init(coordinate:addressDictionary:)

Creates and returns a placemark object using the specified coordinate and Address Book dictionary.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+watchOS 2.0+

``` source
init(
    coordinate: CLLocationCoordinate2D,
    addressDictionary: [String : Any]?
)
```

## Parameters 

`coordinate`  

The geographic coordinate to associate with the placemark.

`addressDictionary`  

A dictionary containing keys and values from an Address Book record. For a list of strings that you can use for the keys of this dictionary, see the “Address Property” constants in `ABPerson`. All of the keys in should be at the top level of the dictionary.

## Return Value

An initialized `MKPlacemark` object.

## Discussion

You can create placemark objects manually for entities for which you already have address information, such as contacts in the Address Book. Creating a placemark object explicitly avoids the need to query the reverse geocoder object for the same information.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Creating a placemark object

init(coordinate: CLLocationCoordinate2D)

Creates and returns a placemark object using the specified coordinate.

init(coordinate: CLLocationCoordinate2D, postalAddress: CNPostalAddress)

Creates and returns a placemark object with the specified coordinate and postal address from the user’s Contacts database.

