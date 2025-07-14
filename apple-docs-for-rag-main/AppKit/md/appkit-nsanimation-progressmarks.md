

- AppKit
- NSAnimation
-  progressMarks 

Instance Property

# progressMarks

An array of floating-point numbers representing current progress marks.

macOS

``` source
var progressMarks: [NSNumber] { get set }
```

## Discussion

The value of this property is an array of NSNumber objects, each of which contains a float value, which are typed to the NSAnimation.Progress type. If there are no progress marks, the array is empty. Setting the value of this property is `nil` clears all progress marks.

## See Also

### Managing Progress Marks

func addProgressMark(NSAnimation.Progress)

Adds the progress mark to the receiver.

func removeProgressMark(NSAnimation.Progress)

Removes progress mark from the receiver.

