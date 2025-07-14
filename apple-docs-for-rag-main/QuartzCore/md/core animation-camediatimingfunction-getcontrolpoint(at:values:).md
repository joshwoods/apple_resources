

- Core Animation
- CAMediaTimingFunction
-  getControlPoint(at:values:) 

Instance Method

# getControlPoint(at:values:)

Returns the control point for the specified index.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func getControlPoint(
    at idx: Int,
    values ptr: UnsafeMutablePointer
)
```

## Parameters 

`idx`  

An integer specifying the index of the control point to return.

`ptr`  

A pointer to an array that, upon return, will contain the x and y values of the specified point.

## Discussion

The value of `index` must be between 0 and 3.

