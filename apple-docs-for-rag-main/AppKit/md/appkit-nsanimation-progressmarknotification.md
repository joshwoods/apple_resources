

- AppKit
- NSAnimation
-  progressMarkNotification 

Type Property

# progressMarkNotification

Posted when the current progress of a running animation reaches one of its progress marks.

macOS

``` source
class let progressMarkNotification: NSNotification.Name
```

## Discussion

The notification object is a running `NSAnimation` object. The `userInfo` dictionary contains the current progress mark, accessed via the key `NSAnimationProgressMark`.

## See Also

### Related Documentation

func animation(NSAnimation, didReachProgressMark: NSAnimation.Progress)

Sent to the delegate when an animation reaches a specific progress mark.

