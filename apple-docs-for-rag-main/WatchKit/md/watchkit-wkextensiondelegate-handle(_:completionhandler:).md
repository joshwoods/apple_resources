

- WatchKit
- WKExtensionDelegate
-  handle(\_:completionHandler:) 

Instance Method

# handle(\_:completionHandler:)

Responds to a Siri intent.

watchOS 5.0+

``` source
@MainActor
optional func handle(
    _ intent: INIntent,
    completionHandler: @escaping (INIntentResponse) -> Void
)
```

``` source
@MainActor
optional func handle(_ intent: INIntent) async -> INIntentResponse
```

## Mentioned in 

Using background tasks

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func handle(_ intent: INIntent) async -> INIntentResponse
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Related Documentation

class WKIntentDidRunRefreshBackgroundTask

A background task used to update your app after a SiriKit intent runs.

