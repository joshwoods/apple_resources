

- UIKit
- UIEvent
- UIEvent.ButtonMask
-  button(\_:) 

Type Method

# button(\_:)

Creates a button mask from the specified button index.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
static func button(_ buttonNumber: Int) -> UIEvent.ButtonMask
```

## Parameters 

`buttonNumber`  

The index of the button on the input device. Pass `1` to represent primary, and `2` to represent secondary.

## See Also

### Creating button masks

init(rawValue: Int)

Creates a button mask with the specified raw value.

