

- WatchKit
- WKInterfaceObject
-  setAccessibilityIdentifier(\_:) 

Instance Method

# setAccessibilityIdentifier(\_:)

Sets the unique identifier string for the interface object.

watchOS

``` source
func setAccessibilityIdentifier(_ accessibilityIdentifier: String?)
```

## Parameters 

`accessibilityIdentifier`  

A string containing the identifier of the element. Specify `nil` to clear the existing identifier.

## Discussion

Use the identifier in this property to distinguish between different objects in your app. The identifier string is used solely for programmatic identity, as opposed to many other accessibility attributes.

## See Also

### Configuring the Accessibility Attributes

func setAccessibilityLabel(String?)

Sets a succinct label on the object that identifies the accessibility element.

func setAccessibilityHint(String?)

Sets the description of what happens when performing an action on the accessibility element.

func setAccessibilityValue(String?)

Sets the value of the accessibility element.

func setIsAccessibilityElement(Bool)

Sets whether the object is an accessibility element that an assistive app can access.

func setAccessibilityTraits(UIAccessibilityTraits)

Sets the combination of accessibility traits that best characterize the accessibility element.

func setAccessibilityImageRegions([WKAccessibilityImageRegion])

Marks portions of an image as separate accessible elements.

