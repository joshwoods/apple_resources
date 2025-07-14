

- Core Location
- CLGeocoder
-  cancelGeocode() 

Instance Method

# cancelGeocode()

Cancels a pending geocoding request.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cancelGeocode()
```

## Discussion

You can use this method to cancel a pending request and free up the resources associated with that request. Canceling a pending request causes the completion handler block to be called.

If the request is not pending, because it has already returned or has not yet begun, this method does nothing.

## See Also

### Managing geocoding requests

var isGeocoding: Bool

A Boolean value indicating whether the receiver is in the middle of geocoding its value.

