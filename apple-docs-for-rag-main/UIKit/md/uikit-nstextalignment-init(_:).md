

- UIKit
- NSTextAlignment
-  init(\_:) 

Initializer

# init(\_:)

Converts a Core Text alignment constant value to the matching constant value in UIKit.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ ctTextAlignment: CTTextAlignment)
```

## Parameters 

`ctTextAlignment`  

The Core Text alignment constant to convert.

## Return Value

The UIKit text alignment that corresponds to the value specified in `ctTextAlignment`.

## Discussion

Use this function when you need to map between the Core Text and UIKit constants for text alignment.

## See Also

### Text manipulations

init(_ nsTextAlignment: NSTextAlignment)

Converts a UIKit text alignment constant value to the matching constant value that Core Text uses.

