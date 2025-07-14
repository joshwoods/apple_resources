

- SwiftUI
-  WritingToolsBehavior 

Structure

# WritingToolsBehavior

The Writing Tools editing experience for text and text input.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.4+

``` source
struct WritingToolsBehavior
```

## Topics

### Type Properties

static let automatic: WritingToolsBehavior

An appropriate editing experience will be provided based on context, which may include disabling the writing tools.

static let complete: WritingToolsBehavior

The complete inline-editing experience is provided if possible.

static let disabled: WritingToolsBehavior

The writing tools are disabled.

static let limited: WritingToolsBehavior

The limited, overlay-panel experience is provided if possible.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Configuring the Writing Tools behavior

func writingToolsBehavior(WritingToolsBehavior) -> some View

Specifies the Writing Tools behavior for text and text input in the environment.

