

- UIKit
- UICalendarSelectionMultiDateDelegate
-  multiDateSelection(\_:didSelectDate:) 

Instance Method

# multiDateSelection(\_:didSelectDate:)

Informs the delegate that a user selected a date represented by date components.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func multiDateSelection(
    _ selection: UICalendarSelectionMultiDate,
    didSelectDate dateComponents: DateComponents
)
```

**Required**

## Parameters 

`selection`  

An object that tracks one or more dates that a user selects from a calendar view.

`dateComponents`  

Date components that represent a date the user selected.

## See Also

### Changing selected dates

func multiDateSelection(UICalendarSelectionMultiDate, didDeselectDate: DateComponents)

Informs the delegate that a user deselected a date represented by date components.

**Required**

