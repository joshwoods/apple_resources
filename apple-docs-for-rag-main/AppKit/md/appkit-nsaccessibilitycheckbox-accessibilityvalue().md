

- AppKit
- NSAccessibilityCheckBox
-  accessibilityValue() 

Instance Method

# accessibilityValue()

Returns the checkbox’s value.

macOS

``` source
func accessibilityValue() -> NSNumber?
```

**Required**

## Return Value

`@YES` if checked; otherwise, `@NO`.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityValue property.

Note

This class must also post an valueChanged notification whenever its value changes.

