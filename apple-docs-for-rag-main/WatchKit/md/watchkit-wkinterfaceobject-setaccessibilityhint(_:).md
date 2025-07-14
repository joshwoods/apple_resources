

- WatchKit
- WKInterfaceObject
-  setAccessibilityHint(\_:) 

Instance Method

# setAccessibilityHint(\_:)

Sets the description of what happens when performing an action on the accessibility element.

watchOS

``` source
func setAccessibilityHint(_ accessibilityHint: String?)
```

## Parameters 

`accessibilityHint`  

A localized string describing what will happen when the user interacts with the object.

## Discussion

Use this method to change the accessibility hint of an object dynamically. You can also set the accessibility hint for an object in Xcode from the Identity inspector.

Follow these guidelines to create a hint for interface objects:

- A hint should be a very brief phrase that begins with a verb that names the result of the action, such as “Dismisses the interface.” To avoid making the hint sound like a command, do not begin the phrase with the imperative form of a verb. For example, do not set the hint to “Dismiss the interface.”

- Do not repeat the action type in the hint. For example, do not create a hint such as “Tap to dismiss the interface.”

- Do not include information about the object involved in the hint. For example, do not create a hint such as “Row that displays details about the item.”

## See Also

### Configuring the Accessibility Attributes

func setAccessibilityIdentifier(String?)

Sets the unique identifier string for the interface object.

func setAccessibilityLabel(String?)

Sets a succinct label on the object that identifies the accessibility element.

func setAccessibilityValue(String?)

Sets the value of the accessibility element.

func setIsAccessibilityElement(Bool)

Sets whether the object is an accessibility element that an assistive app can access.

func setAccessibilityTraits(UIAccessibilityTraits)

Sets the combination of accessibility traits that best characterize the accessibility element.

func setAccessibilityImageRegions([WKAccessibilityImageRegion])

Marks portions of an image as separate accessible elements.

