

- EventKit UI
- EKEventViewController
-  allowsCalendarPreview 

Instance Property

# allowsCalendarPreview

A Boolean that determines whether the user can preview the event in a calendar day.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var allowsCalendarPreview: Bool { get set }
```

## Discussion

If the event is an invitation and this property is true, then a table cell appears allowing the user to preview the event along with other events on the same day. If false (the default), the calendar day preview does not appear. This property applies only to invitations.

## See Also

### Displaying and Editing Event Previews

var allowsEditing: Bool

A Boolean that determines whether the user may edit the event.

