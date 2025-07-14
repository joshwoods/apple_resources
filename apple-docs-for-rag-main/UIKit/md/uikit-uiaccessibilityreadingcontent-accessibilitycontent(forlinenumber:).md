

- UIKit
- UIAccessibilityReadingContent
-  accessibilityContent(forLineNumber:) 

Instance Method

# accessibilityContent(forLineNumber:)

Returns the text associated with the specified line number.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func accessibilityContent(forLineNumber lineNumber: Int) -> String?
```

**Required**

## Parameters 

`lineNumber`  

A line number in the receiver’s content.

## Return Value

A string containing the text that is associated with the specified line number, or `nil` if the line number is invalid. By default, this function returns `nil`.

## Discussion

The system tries to call the accessibilityAttributedContent(forLineNumber:) method before calling this method.

## See Also

### Accessing the content on a page

func accessibilityLineNumber(for: CGPoint) -> Int

Returns the line number that contains the specified point.

**Required**

func accessibilityAttributedContent(forLineNumber: Int) -> NSAttributedString?

Returns the styled text associated with the specified line number.

func accessibilityFrame(forLineNumber: Int) -> CGRect

Returns the onscreen frame associated with the specified line number.

**Required**

func accessibilityAttributedPageContent() -> NSAttributedString?

Returns the styled text displayed on the current page.

func accessibilityPageContent() -> String?

Returns the text displayed on the current page.

**Required**

