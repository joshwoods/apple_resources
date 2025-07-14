

- Network
- nw_parameters_attribution_t
-  nw_parameters_attribution_t.user 

Case

# nw_parameters_attribution_t.user

The user explicitly directs the app to make a network request.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
case user
```

## Mentioned in 

Indicating the source of network activity

## Discussion

Use this value for the `attribution` parameter of a call to the nw_parameters_get_attribution(_:) method when constructing a network request that satisfies a user request to access an explicit, unmodified URL. In all other cases, use the nw_parameters_attribution_t.developer value instead.

## See Also

### Request Sources

case developer

A developer-initiated network request.

