

- Core Location
- CLGeocoder
-  reverseGeocodeLocation(\_:preferredLocale:completionHandler:) 

Instance Method

# reverseGeocodeLocation(\_:preferredLocale:completionHandler:)

Submits a reverse-geocoding request for the specified location and locale.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func reverseGeocodeLocation(
    _ location: CLLocation,
    preferredLocale locale: Locale?,
    completionHandler: @escaping CLGeocodeCompletionHandler
)
```

``` source
func reverseGeocodeLocation(
    _ location: CLLocation,
    preferredLocale locale: Locale?
) async throws -> [CLPlacemark]
```

## Parameters 

`location`  

The location object containing the coordinate data to look up.

`locale`  

The locale to use when returning the address information. You might specify a value for this parameter when you want the address returned in a locale that differs from the user’s current language settings. Specify `nil` to use the user’s default locale information.

`completionHandler`  

The handler block to execute with the results. The geocoder executes this handler regardless of whether the request was successful or unsuccessful. For more information on the format of this block, see CLGeocodeCompletionHandler.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func reverseGeocodeLocation(_ location: CLLocation, preferredLocale locale: Locale?) async throws -> [CLPlacemark]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method submits the specified location data to the geocoding server asynchronously and returns. When the request completes, the geocoder executes the provided completion handler on the main thread.

After initiating a reverse-geocoding request, do not attempt to initiate another reverse- or forward-geocoding request. Geocoding requests are rate-limited for each app, so making too many requests in a short period of time may cause some of the requests to fail. When the maximum rate is exceeded, the geocoder passes an error object with the value network to your completion handler.

## See Also

### Reverse geocoding a location

func reverseGeocodeLocation(CLLocation, completionHandler: CLGeocodeCompletionHandler)

Submits a reverse-geocoding request for the specified location.

typealias CLGeocodeCompletionHandler

A block to be called when a geocoding request is complete.

