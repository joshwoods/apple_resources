

- Core Spotlight
- CSUserQuery
-  CSUserQuery.UserInteractionKind 

Enumeration

# CSUserQuery.UserInteractionKind

Constants that indicate how someone engaged with search-related content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum UserInteractionKind
```

## Topics

### Getting the interaction types

static var `default`: CSUserQuery.UserInteractionKind

case select

case focus

### Creating an interaction kind

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Improving the quality of ranked results

func userEngaged(CSUserQuery.Item, visibleItems: [CSUserQuery.Item], interaction: CSUserQuery.UserInteractionKind)

Notifies the system that someone engaged with a specific search result in your app’s interface.

func userEngaged(CSUserQuery.Suggestion, visibleSuggestions: [CSUserQuery.Suggestion], interaction: CSUserQuery.UserInteractionKind)

Notifies the system that someone engaged with a specific text completion in your app’s interface.

