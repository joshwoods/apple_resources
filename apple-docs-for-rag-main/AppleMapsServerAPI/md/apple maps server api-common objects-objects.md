

- Apple Maps Server API
-  Common objects 

API Collection

# Common objects

Understand the common JSON objects that API responses contain.

## Topics

### Getting an access token

object TokenResponse

An object that contains an access token and an expiration time in seconds.

### Getting common object information

object AutocompleteResult

An object that contains information you can use to suggest addresses and further refine search results.

object DirectionsResponse

An object that describes the directions from a starting location to a destination in terms routes, steps, and a series of waypoints.

object EtaResponse

An object that contains an array of one or more estimated times of arrival (ETAs).

object Location

An object that describes a location in terms of its longitude and latitude.

object MapRegion

An object that describes a map region in terms of its upper-right and lower-left corners as a pair of geographic points.

object Place

An object that describes a place in terms of a variety of spatial, administrative, and qualitative properties.

object PlaceResults

An object that contains an array of places.

object SearchAutocompleteResponse

An array of autocomplete results.

object SearchMapRegion

An object that describes an area to search in terms of its upper-right and lower-left corners as a pair of geographic points.

object SearchResponse

An object that contains the search region and an array of place descriptions that a search returns.

object StructuredAddress

An object that describes the detailed address components of a place.

### Getting common type information

type CountryCode

A string that represents a two-letter country code.

type DirectionsAvoid

A list of the features you can request to avoid when calculating directions.

type Lang

A string that represents a standard tag for identifying languages.

type PoiCategory

A string that describes a specific point of interest (POI) category.

type SearchLocation

A string that describes a geographic location in the form of longitude and latitude.

type SearchRegion

A string that describes a region to search in terms of its upper-right and lower-left corners as a pair of geographic points.

type UserLocation

A string that describes the user’s location in terms of longitude and latitude.

### Handling errors

object ErrorResponse

Information about an error that occurs while processing a request.

## See Also

### Essentials

Creating and using tokens with Maps Server API

Sign JSON Web Tokens to use Maps Server API and debug common signing errors.

Creating a Maps identifier and a private key

Create a Maps identifier and a private key before generating tokens for MapKit JS.

Generate a Maps token

Returns a JWT maps access token that you use to call the service API.

Debugging an Invalid token

Inspect the JavaScript console logs, the token, and events to determine why a token is invalid.

Integrating the Apple Maps Server API into Java server applications

Streamline your app’s API by moving georelated searches from inside your app to your server.

