

- Core Location
- CLGeocoder
-  reverseGeocodeLocation(\_:completionHandler:) 

Instance Method

# reverseGeocodeLocation(\_:completionHandler:)

Submits a reverse-geocoding request for the specified location.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func reverseGeocodeLocation(
    _ location: CLLocation,
    completionHandler: @escaping CLGeocodeCompletionHandler
)
```

``` source
func reverseGeocodeLocation(_ location: CLLocation) async throws -> [CLPlacemark]
```

## Parameters 

`location`  

The location object containing the coordinate data to look up.

`completionHandler`  

The handler block to execute with the results. The geocoder executes this handler regardless of whether the request was successful or unsuccessful. For more information on the format of this block, see CLGeocodeCompletionHandler.

## Mentioned in 

Converting between coordinates and user-friendly place names

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func reverseGeocodeLocation(_ location: CLLocation) async throws -> [CLPlacemark]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method submits the specified location data to the geocoding server asynchronously and returns. When the request completes, the geocoder executes the provided completion handler on the main thread.

After initiating a reverse-geocoding request, do not attempt to initiate another reverse- or forward-geocoding request. Geocoding requests are rate-limited for each app, so making too many requests in a short period of time may cause some of the requests to fail. When the maximum rate is exceeded, the geocoder passes an error object with the value CLError.Code.network to your completion handler.

## See Also

### Reverse geocoding a location

func reverseGeocodeLocation(CLLocation, preferredLocale: Locale?, completionHandler: CLGeocodeCompletionHandler)

Submits a reverse-geocoding request for the specified location and locale.

typealias CLGeocodeCompletionHandler

A block to be called when a geocoding request is complete.

