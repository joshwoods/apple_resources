

- UIKit
- UIProgressView
-  setProgress(\_:animated:) 

Instance Method

# setProgress(\_:animated:)

Adjusts the current progress of the progress view, optionally animating the change.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setProgress(
    _ progress: Float,
    animated: Bool
)
```

## Parameters 

`progress`  

The new progress value.

`animated`  

true if the change should be animated, false if the change should happen immediately.

## Discussion

The current progress is represented by a floating-point value between 0.0 and 1.0, inclusive, where 1.0 indicates the completion of the task. The default value is 0.0. Values less than 0.0 and greater than 1.0 are pinned to those limits.

## See Also

### Managing the progress bar

var progress: Float

The current progress of the progress view.

var observedProgress: Progress?

The progress object to use for updating the progress view.

