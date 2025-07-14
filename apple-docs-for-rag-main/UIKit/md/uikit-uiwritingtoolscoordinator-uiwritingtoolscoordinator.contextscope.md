

- UIKit
- UIWritingToolsCoordinator
-  UIWritingToolsCoordinator.ContextScope 

Enumeration

# UIWritingToolsCoordinator.ContextScope

Options that indicate how much of your content Writing Tools requested.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
enum ContextScope
```

## Overview

At the start of any Writing Tools interaction, you provide the text for the system to evaluate from your UIWritingToolsCoordinator.Delegate object. The request for your content comes with a scope constant that indicates how much of your view’s text to provide.

## Topics

### Getting the scope

case userSelection

An option to provide only the view’s currently selected text.

case fullDocument

An option to provide all of your view’s text.

case visibleArea

An option to provide only the text in the currently visible portion of your view.

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

enum TextReplacementReason

Options that indicate whether Writing Tools is animating changes to your view’s text.

enum TextAnimation

The types of animations that Writing Tools performs during an interactive update of your view.

