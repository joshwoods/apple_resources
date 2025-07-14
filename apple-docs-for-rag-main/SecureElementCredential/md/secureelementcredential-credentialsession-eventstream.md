

- SecureElementCredential
- CredentialSession
-  eventStream 

Instance Property

# eventStream

An asynchronous stream of session events.

iOS 18.1+iPadOS 18.1+

``` source
var eventStream: AsyncStream { get async }
```

## Discussion

Consume and handle events as the session produces then. Do this with a `for-await-in` loop over the stream, like the following example:

```
for await event in session.eventStream {
    // Handle event.
}
```

## See Also

### Handling session events

enum Event

Events produced by a credential session, such as connectivity events and errors.

