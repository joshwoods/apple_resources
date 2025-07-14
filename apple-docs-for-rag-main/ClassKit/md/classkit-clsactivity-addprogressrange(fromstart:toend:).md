

- ClassKit
- CLSActivity
-  addProgressRange(fromStart:toEnd:) 

Instance Method

# addProgressRange(fromStart:toEnd:)

Adds a progress range to a given activity.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
func addProgressRange(
    fromStart start: Double,
    toEnd end: Double
)
```

## Parameters 

`start`  

The beginning of the new range to add. This should be fractional value between 0 and 1, inclusive.

`end`  

The end of the new range to add. This should be larger than the `start` value and less than or equal to one.

## Mentioned in 

Recording student progress

## See Also

### Measuring progress

var progress: Double

A measure of progress through the task, given as a fraction in the range \[0, 1\].

