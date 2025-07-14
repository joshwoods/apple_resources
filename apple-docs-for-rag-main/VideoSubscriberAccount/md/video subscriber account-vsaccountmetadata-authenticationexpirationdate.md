

- Video Subscriber Account
- VSAccountMetadata
-  authenticationExpirationDate 

Instance Property

# authenticationExpirationDate

The date when the user’s current authentication session expires.

iOS 10.0+iPadOS 10.0+macOStvOS 10.0+visionOS 1.0+

``` source
var authenticationExpirationDate: Date? { get }
```

## Discussion

This property is `nil` if the user doesn’t have a current authentication session with their account provider.

## See Also

### Getting TV Provider Info

var accountProviderIdentifier: String?

The unique identifier of the account provider.

