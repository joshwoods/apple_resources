

- SwiftUI
- View
-  accessibilityTextContentType(\_:) 

Instance Method

# accessibilityTextContentType(\_:)

Sets an accessibility text content type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func accessibilityTextContentType(_ value: AccessibilityTextContentType) -> ModifiedContent
```

## Parameters 

`value`  

The accessibility content type from the available AccessibilityTextContentType options.

## Discussion

Use this modifier to set the content type of this accessibility element. Assistive technologies can use this property to choose an appropriate way to output the text. For example, when encountering a source coding context, VoiceOver could choose to speak all punctuation.

The default content type plain.

## See Also

### Describing content

func accessibilityHeading(AccessibilityHeadingLevel) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets the accessibility level of this heading.

enum AccessibilityHeadingLevel

The hierarchy of a heading in relation other headings.

struct AccessibilityTextContentType

Textual context that assistive technologies can use to improve the presentation of spoken text.

