

- PassKit (Apple Pay and Wallet)
- PKIdentityIntentToStore
-  mayStore 

Type Property

# mayStore

An object that indicates your app may store a data element for an indefinite length of time.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class var mayStore: PKIdentityIntentToStore { get }
```

## Mentioned in 

Requesting identity data from a Wallet pass

## See Also

### Getting default intents

class var willNotStore: PKIdentityIntentToStore

An object that indicates your app won’t store a data element any longer than necessary to complete a request.

