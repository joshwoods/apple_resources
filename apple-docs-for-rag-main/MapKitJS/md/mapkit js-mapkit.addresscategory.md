

- MapKit JS
-  mapkit.AddressCategory 

Enumeration

# mapkit.AddressCategory

The categories of address components that users can search for with an address filter.

MapKit JS 5.78.1+

``` source
interface mapkit.AddressCategory {
 const string Country;
 const string AdministrativeArea;
 const string SubAdministrativeArea;
 const string Locality;
 const string SubLocality;
 const string PostalCode;
};
```

## Topics

### Category values

AdministrativeArea

The primary administrative divisions of countries or regions.

Country

Countries and regions.

Locality

Local administrative divisions, postal cities, and populated places.

PostalCode

An address code for mail sorting and delivery.

SubAdministrativeArea

The secondary administrative divisions of countries or regions.

SubLocality

Local administrative subdivisions, postal city subdistricts, and neighborhoods.

## See Also

### Search

mapkit.AddressFilter

An object that filters which address options to include or exclude in search results.

mapkit.Search

An object that retrieves map-based search results for a user-entered query.

