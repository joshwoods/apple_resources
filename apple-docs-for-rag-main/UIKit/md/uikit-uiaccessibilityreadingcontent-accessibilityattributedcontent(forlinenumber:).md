

- UIKit
- UIAccessibilityReadingContent
-  accessibilityAttributedContent(forLineNumber:) 

Instance Method

# accessibilityAttributedContent(forLineNumber:)

Returns the styled text associated with the specified line number.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
optional func accessibilityAttributedContent(forLineNumber lineNumber: Int) -> NSAttributedString?
```

## Parameters 

`lineNumber`  

A line number in the receiver’s content.

## Return Value

An attributed string containing the text that is associated with the specified line number, or `nil` if the line number is invalid. By default, this function returns `nil`.

## Discussion

The system tries to call this method before calling the accessibilityContent(forLineNumber:) method.

## See Also

### Accessing the content on a page

func accessibilityLineNumber(for: CGPoint) -> Int

Returns the line number that contains the specified point.

**Required**

func accessibilityContent(forLineNumber: Int) -> String?

Returns the text associated with the specified line number.

**Required**

func accessibilityFrame(forLineNumber: Int) -> CGRect

Returns the onscreen frame associated with the specified line number.

**Required**

func accessibilityAttributedPageContent() -> NSAttributedString?

Returns the styled text displayed on the current page.

func accessibilityPageContent() -> String?

Returns the text displayed on the current page.

**Required**

