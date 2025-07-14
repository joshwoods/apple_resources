

- AppKit
- NSHapticFeedbackPerformer
-  perform(\_:performanceTime:) 

Instance Method

# perform(\_:performanceTime:)

Initiates a specific pattern of haptic feedback to the user.

macOS 10.11+

``` source
func perform(
    _ pattern: NSHapticFeedbackManager.FeedbackPattern,
    performanceTime: NSHapticFeedbackManager.PerformanceTime
)
```

**Required**

## Parameters 

`pattern`  

A pattern of feedback to be provided to the user. For possible values, see NSHapticFeedbackManager.FeedbackPattern.

`performanceTime`  

The time when the feedback should be provided to the user. For possible values, see NSHapticFeedbackManager.PerformanceTime.

## Discussion

In some cases, the system may override a call to this method. For example, a Force Touch trackpad won’t provide haptic feedback if the user isn’t touching the trackpad.

Important

Call this method only in response to user-initiated actions. Ideally, visual feedback, such as a highlight or appearance of an alignment guide, should accompany the feedback.

## See Also

### Related Documentation

enum PerformanceTime

A time at which to provide haptic feedback to the user.

class NSHapticFeedbackManager

An object that provides access to the haptic feedback management attributes on a system with a Force Touch trackpad.

enum FeedbackPattern

A pattern of haptic feedback to be provided to the user.

