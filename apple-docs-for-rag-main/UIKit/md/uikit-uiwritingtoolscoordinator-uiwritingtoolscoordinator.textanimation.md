

- UIKit
- UIWritingToolsCoordinator
-  UIWritingToolsCoordinator.TextAnimation 

Enumeration

# UIWritingToolsCoordinator.TextAnimation

The types of animations that Writing Tools performs during an interactive update of your view.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
enum TextAnimation
```

## Overview

Use the `UIWritingToolsCoordinator/TextAnimation` constants to determine the type of animation that is occurring. During an interactive change to your view, Writing Tools creates animations to provide feedback about what’s happening. During the setup for each animation, Writing Tools reports the type of animation to the coordinator’s delegate, so that you can perform additional actions related to that animation. For example, during an insertion animation, you might animate changes to other views in your interface.

## Topics

### Getting the animation types

case anticipate

The animation that Writing Tools performs when waiting to receive results from the large language model.

case insert

The animation that Writing Tools performs when inserting text into your view.

case remove

The animation that Writing Tools performs when removing text from your view.

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

enum TextReplacementReason

Options that indicate whether Writing Tools is animating changes to your view’s text.

