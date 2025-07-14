

- Core Location
- CLGeocoder
-  geocodePostalAddress(\_:preferredLocale:completionHandler:) 

Instance Method

# geocodePostalAddress(\_:preferredLocale:completionHandler:)

Submits a forward-geocoding requesting using the specified locale and Contacts framework information.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 4.0+

``` source
func geocodePostalAddress(
    _ postalAddress: CNPostalAddress,
    preferredLocale locale: Locale?,
    completionHandler: @escaping CLGeocodeCompletionHandler
)
```

``` source
func geocodePostalAddress(
    _ postalAddress: CNPostalAddress,
    preferredLocale locale: Locale?
) async throws -> [CLPlacemark]
```

## Parameters 

`postalAddress`  

A postal address from the Contacts framework.

`locale`  

The locale of the postal address. Specify `nil` to use the current locale of the user.

`completionHandler`  

The handler block to execute with the results. The geocoder executes this handler regardless of whether the request was successful or unsuccessful. For more information on the format of this block, see CLGeocodeCompletionHandler.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func geocodePostalAddress(_ postalAddress: CNPostalAddress, preferredLocale locale: Locale?) async throws -> [CLPlacemark]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method submits the specified location data to the geocoding server asynchronously and returns. When the request completes, the geocoder executes the provided completion handler on the main thread.

After initiating a forward-geocoding request, do not attempt to initiate another reverse- or forward-geocoding request. Geocoding requests are rate-limited for each app, so making too many requests in a short period of time may cause some of the requests to fail. When the maximum rate is exceeded, the geocoder passes an error object with the value network to your completion handler.

## See Also

### Geocoding an address

func geocodeAddressString(String, in: CLRegion?, preferredLocale: Locale?, completionHandler: CLGeocodeCompletionHandler)

Submits a forward-geocoding requesting using the specified address string and locale information.

func geocodeAddressString(String, completionHandler: CLGeocodeCompletionHandler)

Submits a forward-geocoding request using the specified string.

func geocodeAddressString(String, in: CLRegion?, completionHandler: CLGeocodeCompletionHandler)

Submits a forward-geocoding request using the specified string and region information.

func geocodePostalAddress(CNPostalAddress, completionHandler: CLGeocodeCompletionHandler)

Submits a forward-geocoding requesting using the specified Contacts framework information.

func geocodeAddressDictionary([AnyHashable : Any], completionHandler: CLGeocodeCompletionHandler)

Submits a forward-geocoding request using the specified address dictionary.

Deprecated

