

- AppKit
- NSAnimation
-  addProgressMark(\_:) 

Instance Method

# addProgressMark(\_:)

Adds the progress mark to the receiver.

macOS

``` source
func addProgressMark(_ progressMark: NSAnimation.Progress)
```

## Parameters 

`progressMark`  

A `float` value (typed as NSAnimationProgress) between 0.0 and 1.0. Values outside that range are pinned to 0.0 or 1.0, whichever is nearest.

## Discussion

A progress mark represents a percentage of the animation completed. When the animation reaches a progress mark, an animation(_:didReachProgressMark:) message is sent to the delegate and an progressMarkNotification is broadcast to all observers. You might receive multiple notifications of progress advances over multiple marks.

## See Also

### Related Documentation

var currentProgress: NSAnimation.Progress

The current progress of the animation.

### Managing Progress Marks

func removeProgressMark(NSAnimation.Progress)

Removes progress mark from the receiver.

var progressMarks: [NSNumber]

An array of floating-point numbers representing current progress marks.

