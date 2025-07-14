

- WatchKit
- WKInterfaceObject
-  setAccessibilityTraits(\_:) 

Instance Method

# setAccessibilityTraits(\_:)

Sets the combination of accessibility traits that best characterize the accessibility element.

watchOS

``` source
func setAccessibilityTraits(_ accessibilityTraits: UIAccessibilityTraits)
```

## Parameters 

`accessibilityTraits`  

The traits that characterize this element. For a list of traits and appropriate combinations, see UIAccessibilityTraits.

## Discussion

Use this method to change the accessibility traits associated with your interface objects.

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

func setIsAccessibilityElement(Bool)

Sets whether the object is an accessibility element that an assistive app can access.

func setAccessibilityImageRegions([WKAccessibilityImageRegion])

Marks portions of an image as separate accessible elements.

