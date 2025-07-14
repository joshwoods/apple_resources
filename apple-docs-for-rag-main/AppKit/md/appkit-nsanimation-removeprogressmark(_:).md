

- AppKit
- NSAnimation
-  removeProgressMark(\_:) 

Instance Method

# removeProgressMark(\_:)

Removes progress mark from the receiver.

macOS

``` source
func removeProgressMark(_ progressMark: NSAnimation.Progress)
```

## Parameters 

`progressMark`  

A `float` value (typed as NSAnimationProgress) that indicates the portion of the animation completed. The value should correspond to a progress mark set with addProgressMark(_:) or NSAnimation.

## See Also

### Managing Progress Marks

func addProgressMark(NSAnimation.Progress)

Adds the progress mark to the receiver.

var progressMarks: [NSNumber]

An array of floating-point numbers representing current progress marks.

