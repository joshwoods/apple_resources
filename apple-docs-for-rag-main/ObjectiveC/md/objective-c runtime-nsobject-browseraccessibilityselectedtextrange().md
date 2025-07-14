

- Objective-C Runtime
- NSObject
-  browserAccessibilitySelectedTextRange() 

Instance Method

# browserAccessibilitySelectedTextRange()

Returns the range of selected text in the element.

iOS 18.0+iPadOS 18.0+macOStvOS 18.0+visionOS 2.0+

``` source
func browserAccessibilitySelectedTextRange() -> NSRange
```

## Return Value

The selection’s range. If there’s no selection, returns `(0,` NSNotFound`)`.

## See Also

### Improving browser accessibility

func browserAccessibilityAttributedValue(in: NSRange) -> NSAttributedString

Returns the value for this element within the given range, as an attributed string.

func browserAccessibilityDeleteTextAtCursor(numberOfCharacters: Int)

Deletes text from the element at the current cursor position.

func browserAccessibilityInsertTextAtCursor(text: String)

Inserts text into the element at the current cursor position.

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

