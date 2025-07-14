

- MapKit JS
-  Place 

Structure

# Place

A place object that returns from a geocoder lookup, a reverse lookup, or a fetch request for points of interest.

MapKit JS 5.0+

``` source
dictionary Place {
 string name;
 string? id;
 string[]? alternateIds;
 mapkit.Coordinate coordinate;
 string formattedAddress;
 mapkit.CoordinateRegion region;
 string countryCode;
 mapkit.PointOfInterestCategory pointOfInterestCategory;
 string? country;
 string? administrativeArea;
 string? administrativeAreaCode;
 string? locality;
 string? postCode;
 string? subLocality;
 string? thoroughfare;
 string? subThoroughfare;
 string? fullThoroughfare;
 string[]? areasOfInterest;
 string[]? dependentLocalities;
};
```

## Overview

GeocoderResponse, SearchResponse, and PointsOfInterestSearchResponse return places.

## Topics

### Place name and category

name

The name of the place.

formattedAddress

The address of the place, formatted using its conventions of its country or region.

areasOfInterest

Common names of the area in which the place resides.

pointOfInterestCategory

The category of the place.

### Street address

thoroughfare

The street name at the place.

subThoroughfare

The number on the street at the place.

fullThoroughfare

A combination of thoroughfare and subthoroughfare.

postCode

The postal code of the place.

### City and district address

locality

The city of the place.

subLocality

The name of the area within the locality.

dependentLocalities

Common names for the local area or neighborhood of the place.

administrativeArea

The state or province of the place.

administrativeAreaCode

The short code for the state or area.

### Country address

country

The country or region of the place.

countryCode

The country or region associated with the place.

### Location

coordinate

The latitude and longitude for the place.

region

The geographic region associated with the place.

### Place IDs

id

The Place ID referencing a feature.

alternateIds

A list of alternate Place IDs referencing a feature.

## See Also

### Places

PlaceDetailOptions

mapkit.PlaceLookup

An object that provides the ability to look up place information for a specified Place ID.

placeDetails

A list of all user-created place detail objects that are currently active on a page.

PlaceLookupOptions

The options for creating a place lookup.

PlaceSelectionAccessoryOptions

The options for selection accessories.

mapkit.PlaceAnnotation

An annotation for a place.

mapkit.PlaceDetail

An interactive view that displays information about a place.

mapkit.PlaceSelectionAccessory

The accessory that conveys information about a place associated with an annotation.

