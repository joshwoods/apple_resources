

- WatchKit
- WKInterfaceObject
-  setAccessibilityValue(\_:) 

Instance Method

# setAccessibilityValue(\_:)

Sets the value of the accessibility element.

watchOS

``` source
func setAccessibilityValue(_ accessibilityValue: String?)
```

## Parameters 

`accessibilityValue`  

The new value for the accessibility element.

## Discussion

When an object has a static label and a dynamic value, set this property to a string that describes the value. For example, a switch object can have a label describing the meaning of the switch, but the value is either On or Off.

## See Also

### Configuring the Accessibility Attributes

func setAccessibilityIdentifier(String?)

Sets the unique identifier string for the interface object.

func setAccessibilityLabel(String?)

Sets a succinct label on the object that identifies the accessibility element.

func setAccessibilityHint(String?)

Sets the description of what happens when performing an action on the accessibility element.

func setIsAccessibilityElement(Bool)

Sets whether the object is an accessibility element that an assistive app can access.

func setAccessibilityTraits(UIAccessibilityTraits)

Sets the combination of accessibility traits that best characterize the accessibility element.

func setAccessibilityImageRegions([WKAccessibilityImageRegion])

Marks portions of an image as separate accessible elements.

