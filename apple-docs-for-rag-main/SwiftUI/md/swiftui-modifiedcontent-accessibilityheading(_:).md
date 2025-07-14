

- SwiftUI
- ModifiedContent
-  accessibilityHeading(\_:) 

Instance Method

# accessibilityHeading(\_:)

Set the level of this heading.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func accessibilityHeading(_ level: AccessibilityHeadingLevel) -> ModifiedContent
```

Available when `Modifier` is `AccessibilityAttachmentModifier`.

## Parameters 

`level`  

The heading level to associate with this element from the available AccessibilityHeadingLevel levels.

## Discussion

Use this modifier to set the level of this heading in relation to other headings. The system speaks the level number of levels AccessibilityHeadingLevel.h1 through AccessibilityHeadingLevel.h6 alongside the text.

The default heading level if you don’t use this modifier is AccessibilityHeadingLevel.unspecified.

