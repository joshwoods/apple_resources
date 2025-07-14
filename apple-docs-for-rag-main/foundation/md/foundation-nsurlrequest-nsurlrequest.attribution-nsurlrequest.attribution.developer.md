

- Foundation
- NSURLRequest
- NSURLRequest.Attribution
-  NSURLRequest.Attribution.developer 

Case

# NSURLRequest.Attribution.developer

A developer-initiated network request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case developer
```

## Discussion

Use this value for the attribution parameter of a URL request that your app makes for any purpose other than when the user explicitly accesses a link. This includes requests that your app makes to get user data. This is the default value.

For cases where the user enters a URL, like in the navigation bar of a web browser, or taps or clicks a URL to load the content it represents, use the NSURLRequest.Attribution.user value instead.

## See Also

### Request sources

case user

The user explicitly directs the app to make a network request.

case user

The user explicitly directs the app to make a network request.

