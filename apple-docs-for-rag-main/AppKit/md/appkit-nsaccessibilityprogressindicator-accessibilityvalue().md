

- AppKit
- NSAccessibilityProgressIndicator
-  accessibilityValue() 

Instance Method

# accessibilityValue()

Returns the progress indicator’s value.

macOS

``` source
func accessibilityValue() -> NSNumber?
```

**Required**

## Return Value

The value of the progress indicator.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityValue property.

Note

This class must also post an valueChanged notification whenever its value changes.

