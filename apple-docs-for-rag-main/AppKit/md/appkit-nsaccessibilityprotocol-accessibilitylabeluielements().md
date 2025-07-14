

- AppKit
- NSAccessibilityProtocol
-  accessibilityLabelUIElements() 

Instance Method

# accessibilityLabelUIElements()

Returns the child label elements for the slider accessibility element.

macOS 10.10+

``` source
func accessibilityLabelUIElements() -> [Any]?
```

**Required**

## See Also

### Configuring Sliders

func accessibilityAllowedValues() -> [NSNumber]?

Returns the allowed values for the slider accessibility element.

**Required**

func setAccessibilityAllowedValues([NSNumber]?)

Sets the allowed values for the slider accessibility element.

**Required**

func setAccessibilityLabelUIElements([Any]?)

Sets the child label elements for the slider accessibility element.

**Required**

func accessibilityLabelValue() -> Float

Returns the value of the label accessibility element.

**Required**

func setAccessibilityLabelValue(Float)

Sets the value of the label accessibility element.

**Required**

