

- WatchKit
- WKInterfaceObject
-  setAccessibilityImageRegions(\_:) 

Instance Method

# setAccessibilityImageRegions(\_:)

Marks portions of an image as separate accessible elements.

watchOS

``` source
func setAccessibilityImageRegions(_ accessibilityImageRegions: [WKAccessibilityImageRegion])
```

## Parameters 

`accessibilityImageRegions`  

An array of WKAccessibilityImageRegion objects. Each object in the array represents a portion of the interface object’s foreground or background image that should be treated as a separate accessible element.

## Discussion

Use this method to associate different accessibility labels with different parts of the object’s image. You might also use this method to assign accessibility information to different parts of a dynamically generated image.

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

func setAccessibilityTraits(UIAccessibilityTraits)

Sets the combination of accessibility traits that best characterize the accessibility element.

