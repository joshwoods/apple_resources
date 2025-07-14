

- Core ML
-  MLUpdateProgressEvent 

Structure

# MLUpdateProgressEvent

A type of event during a model update task.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
struct MLUpdateProgressEvent
```

## Topics

### Getting Progress Event Types

static var trainingBegin: MLUpdateProgressEvent

An event that represents the start of training.

static var miniBatchEnd: MLUpdateProgressEvent

An event that represents the end of a mini-batch within a training epoch.

static var epochEnd: MLUpdateProgressEvent

An event that represents the end of training epoch.

### Creating a Progress Event

init(rawValue: Int)

Creates a progress event for the given integer.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Getting the Update Context

var event: MLUpdateProgressEvent

The event type that triggered an update task to notify your app’s completion and update progress handlers.

var task: MLUpdateTask

The update task that generated the update context.

var parameters: [MLParameterKey : Any]

The parameters for the update task.

class MLParameterKey

The keys for the parameter dictionary in a model configuration or a model update context.

