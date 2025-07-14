

- Create ML
- MLRandomForestClassifier
-  restoreTrainingSession(sessionParameters:) 

Type Method

# restoreTrainingSession(sessionParameters:)

Restores an existing training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
static func restoreTrainingSession(sessionParameters: MLTrainingSessionParameters) throws -> MLTrainingSession
```

## Parameters 

`sessionParameters`  

Training session parameters. The `sessionDirectory` parameter is required.

## Return Value

A `MLTrainingSession` that can be used to resume training.

