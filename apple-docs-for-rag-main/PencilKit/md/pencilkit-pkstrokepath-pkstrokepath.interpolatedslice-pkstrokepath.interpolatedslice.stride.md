

- PencilKit
- PKStrokePath
- PKStrokePath.InterpolatedSlice
-  PKStrokePath.InterpolatedSlice.Stride 

Enumeration

# PKStrokePath.InterpolatedSlice.Stride

The stride between elements of this slice.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
enum Stride
```

## Topics

### Stride types

case distance(CGFloat)

A stride based on a distance between elements you provide.

case parametricStep(CGFloat)

A stride based on a parametric step value you provide.

case time(TimeInterval)

A stride based on a time interval in seconds you provide.

