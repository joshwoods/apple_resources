

- Core Location
- CLGeocoder
-  geocodeAddressDictionary(\_:completionHandler:) Deprecated

Instance Method

# geocodeAddressDictionary(\_:completionHandler:)

Submits a forward-geocoding request using the specified address dictionary.

iOS 5.0–11.0DeprecatediPadOS 5.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.13DeprecatedtvOS 9.0–11.0DeprecatedwatchOS 1.0–4.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, watchOS**

``` source
func geocodeAddressDictionary(
    _ addressDictionary: [AnyHashable : Any],
    completionHandler: @escaping CLGeocodeCompletionHandler
)
```

**Mac Catalyst**

``` source
func geocodeAddressDictionary(_ addressDictionary: [AnyHashable : Any]) async throws -> [CLPlacemark]
```

Deprecated

Use geocodePostalAddress(_:preferredLocale:completionHandler:) or geocodePostalAddress(_:completionHandler:) instead.

## Parameters 

`addressDictionary`  

An Address Book dictionary containing information about the address to look up.

`completionHandler`  

A block object containing the code to execute at the end of the request. This code is called whether the request is successful or unsuccessful.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method submits the specified location data to the geocoding server asynchronously and returns. Your completion handler block will be executed on the main thread.

After initiating a forward-geocoding request, do not attempt to initiate another forward- or reverse-geocoding request. Geocoding requests are rate-limited for each app, so making too many requests in a short period of time may cause some of the requests to fail. When the maximum rate is exceeded, the geocoder passes an error object with the value CLError.Code.network to your completion handler.

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

func geocodePostalAddress(CNPostalAddress, preferredLocale: Locale?, completionHandler: CLGeocodeCompletionHandler)

Submits a forward-geocoding requesting using the specified locale and Contacts framework information.

