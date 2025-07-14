

- PassKit (Apple Pay and Wallet)
- PKIdentityAuthorizationController
-  cancelRequest() 

Instance Method

# cancelRequest()

Cancels a request in progress.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
func cancelRequest()
```

## Discussion

Use this method to cancel an in progress request. Cancellation isn’t guarenteed when you call this method, the system might return a document response if it was already in flight.

