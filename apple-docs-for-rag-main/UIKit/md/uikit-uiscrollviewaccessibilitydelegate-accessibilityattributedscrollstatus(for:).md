

- UIKit
- UIScrollViewAccessibilityDelegate
-  accessibilityAttributedScrollStatus(for:) 

Instance Method

# accessibilityAttributedScrollStatus(for:)

Returns an attributed string describing the content at the current offset in the scroll view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
optional func accessibilityAttributedScrollStatus(for scrollView: UIScrollView) -> NSAttributedString?
```

## Parameters 

`scrollView`  

The scroll view containing the content.

## Return Value

An attributed string describing the content.

## Discussion

Your implementation of this method returns a description of the content that’s currently visible in the scroll view. Use this method (instead of the accessibilityScrollStatus(for:) method) when you want to include attributes that specify which language to use when speaking the text. For more information, see accessibilitySpeechLanguage (Swift) or UIAccessibilitySpeechAttributeLanguage (Objective-C).

## See Also

### Providing descriptive information

func accessibilityScrollStatus(for: UIScrollView) -> String?

Returns a string describing the content at the current offset in the scroll view.

