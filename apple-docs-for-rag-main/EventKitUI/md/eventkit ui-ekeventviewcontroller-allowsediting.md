

- EventKit UI
- EKEventViewController
-  allowsEditing 

Instance Property

# allowsEditing

A Boolean that determines whether the user may edit the event.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var allowsEditing: Bool { get set }
```

## Discussion

If false (the default), the event is not editable. If true, an Edit button appears, allowing the user to change properties of the event. This property applies only to events in calendars created by the user. For example, it doesn’t apply to invitations sent by another user.

## See Also

### Displaying and Editing Event Previews

var allowsCalendarPreview: Bool

A Boolean that determines whether the user can preview the event in a calendar day.

