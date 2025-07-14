

- UIKit
- UIAccessibilityReadingContent
-  accessibilityAttributedPageContent() 

Instance Method

# accessibilityAttributedPageContent()

Returns the styled text displayed on the current page.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
optional func accessibilityAttributedPageContent() -> NSAttributedString?
```

## Return Value

An attributed string that contains the text displayed on the current page.

## Discussion

The system tries to call this method before calling the accessibilityPageContent() method.

## See Also

### Accessing the content on a page

func accessibilityLineNumber(for: CGPoint) -> Int

Returns the line number that contains the specified point.

**Required**

func accessibilityAttributedContent(forLineNumber: Int) -> NSAttributedString?

Returns the styled text associated with the specified line number.

func accessibilityContent(forLineNumber: Int) -> String?

Returns the text associated with the specified line number.

**Required**

func accessibilityFrame(forLineNumber: Int) -> CGRect

Returns the onscreen frame associated with the specified line number.

**Required**

func accessibilityPageContent() -> String?

Returns the text displayed on the current page.

**Required**

