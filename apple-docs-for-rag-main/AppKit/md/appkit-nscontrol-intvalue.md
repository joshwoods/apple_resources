

- AppKit
- NSControl
-  intValue 

Instance Property

# intValue

The value of the receiver’s cell as an integer.

macOS

``` source
@MainActor
var intValue: Int32 { get set }
```

## Discussion

If the control contains many cells (for example, `NSMatrix`), then this property contains the value of the currently selected cell. If the control is in the process of editing the affected cell, then it invokes the validateEditing() method before getting the value.

If the cell is being edited, setting this property aborts all editing before setting the value. If the cell does not inherit from `NSActionCell`, setting this property marks the cell’s interior as needing to be redisplayed; `NSActionCell` performs its own updating of cells.

## See Also

### Accessing the Control’s Value

var doubleValue: Double

The value of the receiver’s cell as a double-precision floating-point number.

var floatValue: Float

The value of the receiver’s cell as a single-precision floating-point number.

var integerValue: Int

The value of the receiver’s cell as an NSInteger value.

var objectValue: Any?

The value of the receiver’s cell as an Objective-C object.

var stringValue: String

The value of the receiver’s cell as an `NSString` object.

var attributedStringValue: NSAttributedString

The value of the receiver’s cell as an attributed string.

