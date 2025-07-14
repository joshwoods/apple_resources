

- Core Location
-  CLGeocodeCompletionHandler 

Type Alias

# CLGeocodeCompletionHandler

A block to be called when a geocoding request is complete.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias CLGeocodeCompletionHandler = ([CLPlacemark]?, (any Error)?) -> Void
```

## Discussion

Upon completion of a geocoding request, a block of this form is called to give you a chance to process the results. The parameters of this block are as follows:

`placemark`  
Contains an array of CLPlacemark objects. For most geocoding requests, this array should contain only one entry. However, forward-geocoding requests may return multiple placemark objects in situations where the specified address could not be resolved to a single location.

If the request was canceled or there was an error in obtaining the placemark information, this parameter is `nil`.

`error`  
Contains `nil` or an error object indicating why the placemark data was not returned. For a list of possible error codes, see CLError.Code.

## See Also

### Reverse geocoding a location

func reverseGeocodeLocation(CLLocation, preferredLocale: Locale?, completionHandler: CLGeocodeCompletionHandler)

Submits a reverse-geocoding request for the specified location and locale.

func reverseGeocodeLocation(CLLocation, completionHandler: CLGeocodeCompletionHandler)

Submits a reverse-geocoding request for the specified location.

