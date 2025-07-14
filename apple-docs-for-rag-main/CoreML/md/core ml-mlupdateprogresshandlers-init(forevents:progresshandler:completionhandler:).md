

- Core ML
- MLUpdateProgressHandlers
-  init(forEvents:progressHandler:completionHandler:) 

Initializer

# init(forEvents:progressHandler:completionHandler:)

Creates the collection of closures an update task uses to notify your app of its progress.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    forEvents interestedEvents: MLUpdateProgressEvent,
    progressHandler: ((MLUpdateContext) -> Void)?,
    completionHandler: @escaping (MLUpdateContext) -> Void
)
```

## Parameters 

`interestedEvents`  

The events for which the update task will call your closures for, contained in an option set.

`progressHandler`  

The closure an update task uses to notify your app. The update task only uses this closure for the events you specified in `interestedEvents`.

`completionHandler`  

The closure that an update tasks uses to notify you when it is complete.

## See Also

### Creating Progress Handlers

struct MLUpdateProgressEvent

A type of event during a model update task.

class MLUpdateContext

The context an update task provides to your app’s completion and update progress handlers.

