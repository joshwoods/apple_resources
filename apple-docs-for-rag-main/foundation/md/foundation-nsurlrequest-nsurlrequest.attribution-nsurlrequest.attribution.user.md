

- Foundation
- NSURLRequest
- NSURLRequest.Attribution
-  NSURLRequest.Attribution.user 

Case

# NSURLRequest.Attribution.user

The user explicitly directs the app to make a network request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case user
```

## Discussion

Use this value for the attribution parameter of a URL request that satisfies a user request to access an explicit, unmodified URL. In all other cases, use the NSURLRequest.Attribution.developer value instead.

## See Also

### Request sources

case developer

A developer-initiated network request.

case developer

A developer-initiated network request.

