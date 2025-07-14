

- Core ML
- MLUpdateProgressEvent
-  epochEnd 

Type Property

# epochEnd

An event that represents the end of training epoch.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
static var epochEnd: MLUpdateProgressEvent { get }
```

## See Also

### Getting Progress Event Types

static var trainingBegin: MLUpdateProgressEvent

An event that represents the start of training.

static var miniBatchEnd: MLUpdateProgressEvent

An event that represents the end of a mini-batch within a training epoch.

