

- WatchKit
- WKApplicationDelegate
-  handle(\_:completionHandler:) 

Instance Method

# handle(\_:completionHandler:)

Responds to a Siri intent.

watchOS 7.0+

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

## Parameters 

`intent`  

An intent containing information about the user’s request.

`completionHandler`  

A closure that you call as soon as you finish handling the intent.

## Discussion

The system calls this method when it receives a Siri intent. Implement a method that handles the incoming intent, and then call the completion handler as quickly as possible.

## See Also

### Related Documentation

class WKIntentDidRunRefreshBackgroundTask

A background task used to update your app after a SiriKit intent runs.

