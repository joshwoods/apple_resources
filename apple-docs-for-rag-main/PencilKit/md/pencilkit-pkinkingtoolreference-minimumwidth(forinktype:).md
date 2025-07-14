

- PencilKit
- PKInkingToolReference
-  minimumWidth(forInkType:) 

Type Method

# minimumWidth(forInkType:)

Returns the minimum allowed line width for the specified tool type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class func minimumWidth(forInkType inkType: __PKInkType) -> CGFloat
```

## Parameters 

`inkType`  

The type of tool whose minimum line width you want.

## Return Value

The minimum line width (in points) for the specified tool type.

## See Also

### Getting the standard ink widths

class func defaultWidth(forInkType: __PKInkType) -> CGFloat

Returns the default line width for the specified tool type.

class func maximumWidth(forInkType: __PKInkType) -> CGFloat

Returns the maximum allowed line width for the specified tool type.

