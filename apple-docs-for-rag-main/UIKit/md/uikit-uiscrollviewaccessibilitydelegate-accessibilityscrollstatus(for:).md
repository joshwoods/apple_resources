

- UIKit
- UIScrollViewAccessibilityDelegate
-  accessibilityScrollStatus(for:) 

Instance Method

# accessibilityScrollStatus(for:)

Returns a string describing the content at the current offset in the scroll view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func accessibilityScrollStatus(for scrollView: UIScrollView) -> String?
```

## Parameters 

`scrollView`  

The scroll view containing the content.

## Return Value

A custom status string for the current offset.

## Discussion

For example, in a user interface that scrolls through the books in a bookcase, you could return “Books 10 through 20”. By default, VoiceOver announces “Page *X* of *Y*” while scrolling.

Use the accessibilityAttributedScrollStatus(for:) method if portions of your string should be spoken in a different language.

## See Also

### Providing descriptive information

func accessibilityAttributedScrollStatus(for: UIScrollView) -> NSAttributedString?

Returns an attributed string describing the content at the current offset in the scroll view.

