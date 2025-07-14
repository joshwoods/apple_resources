

- Core ML
- MLUpdateContext
-  task 

Instance Property

# task

The update task that generated the update context.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
var task: MLUpdateTask { get }
```

## See Also

### Getting the Update Context

var event: MLUpdateProgressEvent

The event type that triggered an update task to notify your app’s completion and update progress handlers.

struct MLUpdateProgressEvent

A type of event during a model update task.

var parameters: [MLParameterKey : Any]

The parameters for the update task.

class MLParameterKey

The keys for the parameter dictionary in a model configuration or a model update context.

