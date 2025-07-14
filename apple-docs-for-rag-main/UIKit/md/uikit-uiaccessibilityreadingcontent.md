

- UIKit
-  UIAccessibilityReadingContent 

Protocol

# UIAccessibilityReadingContent

Methods to implement for an object that represents content that users read, such as a book or an article.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
protocol UIAccessibilityReadingContent
```

## Overview

To give VoiceOver users a superior, continuous reading experience, you can implement this protocol on an element that represents readable content, characterize it with the causesPageTurn trait, and use the UIAccessibilityScrollDirection.next and UIAccessibilityScrollDirection.previous constants to enable page turning.

## Topics

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

func accessibilityPageContent() -> String?

Returns the text displayed on the current page.

**Required**

## See Also

### Behaviors

UIAccessibilityFocus

An informal protocol that provides a way to determine whether an assistive app, such as VoiceOver, has focus on an accessible element.

protocol UIAccessibilityIdentification

Methods that associate a unique identifier with elements in your user interface.

protocol UIAccessibilityContentSizeCategoryImageAdjusting

Methods to determine when to adjust images for different content size categories.

struct UIAccessibilityTextualContext

Constants that describe a named context that helps identify and classify the type of text inside an element.

