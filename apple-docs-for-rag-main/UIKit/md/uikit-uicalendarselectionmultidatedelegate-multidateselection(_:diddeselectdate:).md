

- UIKit
- UICalendarSelectionMultiDateDelegate
-  multiDateSelection(\_:didDeselectDate:) 

Instance Method

# multiDateSelection(\_:didDeselectDate:)

Informs the delegate that a user deselected a date represented by date components.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func multiDateSelection(
    _ selection: UICalendarSelectionMultiDate,
    didDeselectDate dateComponents: DateComponents
)
```

**Required**

## Parameters 

`selection`  

An object that tracks multiple dates that a user selects from a calendar view.

`dateComponents`  

Date components that represent a date the user deselected.

## See Also

### Changing selected dates

func multiDateSelection(UICalendarSelectionMultiDate, didSelectDate: DateComponents)

Informs the delegate that a user selected a date represented by date components.

**Required**

