

- Network
- nw_parameters_attribution_t
-  nw_parameters_attribution_t.developer 

Case

# nw_parameters_attribution_t.developer

A developer-initiated network request.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
case developer
```

## Discussion

Use this value for the `attribution` parameter of a call to the nw_parameters_get_attribution(_:) method when creating a network request for any purpose other than when the user explicitly accesses a link. This includes requests that your app makes to get user data. This is the default value.

For cases where the user enters a URL, like in the navigation bar of a web browser, or taps or clicks a URL to load the content it represents, use the nw_parameters_attribution_t.user value instead.

## See Also

### Request Sources

case user

The user explicitly directs the app to make a network request.

