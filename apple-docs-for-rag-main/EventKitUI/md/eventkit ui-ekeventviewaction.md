

- EventKit UI
-  EKEventViewAction 

Enumeration

# EKEventViewAction

Describes the action taken to close the event view controller.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
enum EKEventViewAction
```

## Topics

### Constants

case done

The user tapped the Done button.

case responded

The user responded to and saved a pending event invitation.

case deleted

The user deleted the event.

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

### Responding to the Interface’s Dismissal

func eventViewController(EKEventViewController, didCompleteWith: EKEventViewAction)

Invoked when closing the event view controller.

**Required**

