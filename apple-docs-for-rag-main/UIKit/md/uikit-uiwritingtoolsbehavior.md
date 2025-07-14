

- UIKit
-  UIWritingToolsBehavior 

Enumeration

# UIWritingToolsBehavior

Constants that specify the writing tools experience for the underlying view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.4+

``` source
enum UIWritingToolsBehavior
```

## Overview

Writing tools provide proofreading and rewriting support for the content of text views. On devices that support writing tools features, people engage the system UI to choose how to rewrite all or part of the available text. These constants indicate whether people experience writing tools inline with their text, in an overlay panel, or not at all.

## Topics

### Getting the writing tools behaviors

case none

An option to prevent the writing tools from modifying the text in the view.

case `default`

An option to let the system determine the best way to enable writing tools for the view.

case complete

An option to provide the complete writing tools experience for the text view.

case limited

An option to provide a limited, overlay-panel experience for the text view.

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

### Configuration

Customizing Writing Tools behavior for UIKit views

Modify the behavior of Writing Tools in standard iOS text views, and adjust your app’s behavior while the feature is active.

struct UIWritingToolsResultOptions

Constants to specify what type of content to allow in Writing Tools suggestions or rewrites.

