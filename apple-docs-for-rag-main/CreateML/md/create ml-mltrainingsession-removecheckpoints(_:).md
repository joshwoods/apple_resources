

- Create ML
- MLTrainingSession
-  removeCheckpoints(\_:) 

Instance Method

# removeCheckpoints(\_:)

Removes the checkpoints that satisfy your closure from the training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
final func removeCheckpoints(_ predicate: (MLCheckpoint) -> Bool) throws
```

## Discussion

- predicate: A closure that returns a Boolean indicating whether to remove a checkpoint.

