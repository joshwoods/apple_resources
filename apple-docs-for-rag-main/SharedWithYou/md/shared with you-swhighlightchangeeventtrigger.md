

- Shared With You
-  SWHighlightChangeEventTrigger 

Enumeration

# SWHighlightChangeEventTrigger

The type of change event for the highlight

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
enum SWHighlightChangeEventTrigger
```

## Mentioned in 

Adding shared content collaboration to your app

## Topics

### Change actions

case edit

Signifies a highlight edit.

case comment

Signifies a highlight comment.

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

### Accessing event attributes

var highlightURL: URL

The URL of the hightlight.

var changeEventTrigger: SWHighlightChangeEventTrigger

The type of change event for the highlight.

