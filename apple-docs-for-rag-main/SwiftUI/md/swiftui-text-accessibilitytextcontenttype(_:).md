

- SwiftUI
- Text
-  accessibilityTextContentType(\_:) 

Instance Method

# accessibilityTextContentType(\_:)

Sets an accessibility text content type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func accessibilityTextContentType(_ value: AccessibilityTextContentType) -> Text
```

## Parameters 

`value`  

The accessibility content type from the available AccessibilityTextContentType options.

## Discussion

Use this modifier to set the content type of this accessibility element. Assistive technologies can use this property to choose an appropriate way to output the text. For example, when encountering a source coding context, VoiceOver could choose to speak all punctuation.

If you don’t set a value with this method, the default content type is plain.

## See Also

### Providing accessibility information

func accessibilityHeading(AccessibilityHeadingLevel) -> Text

Sets the accessibility level of this heading.

func accessibilityLabel(_:)

Adds a label to the view that describes its contents.

