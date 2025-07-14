

- AppKit
- NSAccessibilityProtocol
-  setAccessibilityAllowedValues(\_:) 

Instance Method

# setAccessibilityAllowedValues(\_:)

Sets the allowed values for the slider accessibility element.

macOS 10.10+

``` source
func setAccessibilityAllowedValues(_ accessibilityAllowedValues: [NSNumber]?)
```

**Required**

## See Also

### Configuring Sliders

func accessibilityAllowedValues() -> [NSNumber]?

Returns the allowed values for the slider accessibility element.

**Required**

func accessibilityLabelUIElements() -> [Any]?

Returns the child label elements for the slider accessibility element.

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

