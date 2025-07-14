

- UIKit
- UIWritingToolsCoordinator
-  UIWritingToolsCoordinator.TextReplacementReason 

Enumeration

# UIWritingToolsCoordinator.TextReplacementReason

Options that indicate whether Writing Tools is animating changes to your view’s text.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
enum TextReplacementReason
```

## Overview

During an operation, Writing Tools delivers replacement text to the delegate of the active UIWritingToolsCoordinator object. Depending on the configured experience for your view, it delivers these changes as either interactive or noninteractive replacements. For interactive replacements, Writing Tools animates the change automatically and provides you with the information you need to perform any related animations.

## Topics

### Getting the reasons

case interactive

An option to animate the replacement of text in your view.

case noninteractive

An option to replace the text in your view without animating the change.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the supporting types

enum ContextScope

Options that indicate how much of your content Writing Tools requested.

enum TextAnimation

The types of animations that Writing Tools performs during an interactive update of your view.

