

- UIKit
- UICalendarView
- UICalendarView.Decoration
-  customView(\_:) 

Type Method

# customView(\_:)

Creates a new calendar view decoration with a custom view, using your view provider.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
class func customView(_ customViewProvider: @escaping () -> UIView) -> Self
```

## Parameters 

`customViewProvider`  

A block of code that creates and returns a calendar view decoration.

## Return Value

A calendar view decoration.

## Discussion

Create and return a decoration view for the calendar view in your `customViewProvider` block. The calendar view will clip the decoration view to its parent’s bounds. The decoration view may not have any interactions.

