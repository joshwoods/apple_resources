

- Objective-C Runtime
- NSObject
-  browserAccessibilityAttributedValue(in:) 

Instance Method

# browserAccessibilityAttributedValue(in:)

Returns the value for this element within the given range, as an attributed string.

iOS 18.0+iPadOS 18.0+macOStvOS 18.0+visionOS 2.0+

``` source
func browserAccessibilityAttributedValue(in range: NSRange) -> NSAttributedString
```

## Parameters 

`range`  

The range within this element’s value to return.

## Return Value

An attributed string that’s the substring of this element’s value within the given range.

## See Also

### Improving browser accessibility

func browserAccessibilityDeleteTextAtCursor(numberOfCharacters: Int)

Deletes text from the element at the current cursor position.

func browserAccessibilityInsertTextAtCursor(text: String)

Inserts text into the element at the current cursor position.

func browserAccessibilitySelectedTextRange() -> NSRange

Returns the range of selected text in the element.

func browserAccessibilitySetSelectedTextRange(NSRange)

Updates the element’s selected text.

func browserAccessibilityValue(in: NSRange) -> String

Returns this element’s value in the given range.

var browserAccessibilityContainerType: BEAccessibilityContainerType

The kind of container that contains this element.

var browserAccessibilityCurrentStatus: String?

A string that’s the element’s value for aria-current.

var browserAccessibilityHasDOMFocus: Bool

A Boolean value that indicates whether the element has native focus in the browser Document Object Model.

var browserAccessibilityIsRequired: Bool

A Boolean value that’s the element’s value for aria-required.

var browserAccessibilityPressedState: BEAccessibilityPressedState

The element’s value for aria-pressed.

var browserAccessibilityRoleDescription: String?

A string that describes the element’s role for assistive technologies.

var browserAccessibilitySortDirection: String?

A string that’s the element’s value for aria-sort.

