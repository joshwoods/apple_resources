

- SwiftUI
- AnimationCompletionCriteria
-  removed 

Type Property

# removed

The entire animation is finished and will now be removed.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static let removed: AnimationCompletionCriteria
```

## Discussion

If a subsequent change occurs that creates additional animations on properties with `removed` completion callbacks registered, then those callbacks will only fire when *all* of the created animations are complete.

## See Also

### Getting the completion criteria

static let logicallyComplete: AnimationCompletionCriteria

The animation has logically completed, but may still be in its long tail.

