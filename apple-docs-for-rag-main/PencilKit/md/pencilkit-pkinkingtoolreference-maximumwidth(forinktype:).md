

- PencilKit
- PKInkingToolReference
-  maximumWidth(forInkType:) 

Type Method

# maximumWidth(forInkType:)

Returns the maximum allowed line width for the specified tool type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class func maximumWidth(forInkType inkType: __PKInkType) -> CGFloat
```

## Parameters 

`inkType`  

The type of tool whose maximum line width you want.

## Return Value

The maximum line width (in points) for the specified tool type.

## See Also

### Getting the standard ink widths

class func defaultWidth(forInkType: __PKInkType) -> CGFloat

Returns the default line width for the specified tool type.

class func minimumWidth(forInkType: __PKInkType) -> CGFloat

Returns the minimum allowed line width for the specified tool type.

