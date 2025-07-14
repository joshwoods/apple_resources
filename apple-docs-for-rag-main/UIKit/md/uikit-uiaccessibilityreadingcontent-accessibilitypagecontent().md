

- UIKit
- UIAccessibilityReadingContent
-  accessibilityPageContent() 

Instance Method

# accessibilityPageContent()

Returns the text displayed on the current page.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func accessibilityPageContent() -> String?
```

**Required**

## Return Value

A string that contains the text displayed on the current page.

## Discussion

The system tries to call the accessibilityAttributedPageContent() method before calling this method.

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

func accessibilityAttributedPageContent() -> NSAttributedString?

Returns the styled text displayed on the current page.

