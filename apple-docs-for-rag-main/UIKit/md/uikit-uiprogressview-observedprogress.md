

- UIKit
- UIProgressView
-  observedProgress 

Instance Property

# observedProgress

The progress object to use for updating the progress view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var observedProgress: Progress? { get set }
```

## Discussion

When this property is set, the progress view updates its progress value automatically using information it receives from the Progress object. (Progress updates are animated.) Set the property to `nil` when you want to update the progress manually. The default value of this property is `nil`.

For more information about configuring a progress object to manage progress information, see Progress.

## See Also

### Managing the progress bar

var progress: Float

The current progress of the progress view.

func setProgress(Float, animated: Bool)

Adjusts the current progress of the progress view, optionally animating the change.

