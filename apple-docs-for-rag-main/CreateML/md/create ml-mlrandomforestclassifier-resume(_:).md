

- Create ML
- MLRandomForestClassifier
-  resume(\_:) 

Type Method

# resume(\_:)

Resumes a training session from the last checkpoint if available.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
static func resume(_ session: MLTrainingSession) throws -> MLJob
```

## Parameters 

`session`  

Loaded or new training session.

## Return Value

A `MLJob` that can be used to observe training progress.

## Discussion

If there are no resumable checkpoints training starts over from the beginning.

