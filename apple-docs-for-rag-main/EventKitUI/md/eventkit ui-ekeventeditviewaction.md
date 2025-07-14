

- EventKit UI
-  EKEventEditViewAction 

Enumeration

# EKEventEditViewAction

The action taken by the user after editing an event.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
enum EKEventEditViewAction
```

## Topics

### Constants

case canceled

The user canceled changes made to the event.

case saved

The user saved changes made to the event.

case deleted

The user deleted the event.

static var cancelled: EKEventEditViewAction

A static variable used to cancel changes made to the event.

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

### Finishing an Edit

func eventEditViewController(EKEventEditViewController, didCompleteWith: EKEventEditViewAction)

Invoked when the user finishes editing an event.

**Required**

