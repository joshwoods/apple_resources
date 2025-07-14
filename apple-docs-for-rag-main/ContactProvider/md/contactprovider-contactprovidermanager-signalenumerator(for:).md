

- ContactProvider
- ContactProviderManager
-  signalEnumerator(for:) 

Instance Method

# signalEnumerator(for:)

Requests that the extension enumerate its contacts for the domain.

iOS 18.0+iPadOS 18.0+

``` source
func signalEnumerator(for collection: ContactItem.Identifier = .rootContainer) async throws
```

## Parameters 

`collection`  

The collection to enumerate; defaults to rootContainer.

## Discussion

You typically call this when you need to invoke the app extension on demand. One example is when the app receives a push notification informing it that updated contact data is available.

