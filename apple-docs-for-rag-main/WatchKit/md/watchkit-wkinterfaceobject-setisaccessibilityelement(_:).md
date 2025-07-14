

- WatchKit
- WKInterfaceObject
-  setIsAccessibilityElement(\_:) 

Instance Method

# setIsAccessibilityElement(\_:)

Sets whether the object is an accessibility element that an assistive app can access.

watchOS

``` source
func setIsAccessibilityElement(_ isAccessibilityElement: Bool)
```

## Parameters 

`isAccessibilityElement`  

true if the object is an accessibility element or false if it is not.

## Discussion

Use this method to change the accessibility status of your interface objects.

## See Also

### Configuring the Accessibility Attributes

func setAccessibilityIdentifier(String?)

Sets the unique identifier string for the interface object.

func setAccessibilityLabel(String?)

Sets a succinct label on the object that identifies the accessibility element.

func setAccessibilityHint(String?)

Sets the description of what happens when performing an action on the accessibility element.

func setAccessibilityValue(String?)

Sets the value of the accessibility element.

func setAccessibilityTraits(UIAccessibilityTraits)

Sets the combination of accessibility traits that best characterize the accessibility element.

func setAccessibilityImageRegions([WKAccessibilityImageRegion])

Marks portions of an image as separate accessible elements.

