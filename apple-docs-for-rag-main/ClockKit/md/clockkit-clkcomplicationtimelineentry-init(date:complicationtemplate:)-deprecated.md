

- ClockKit
- CLKComplicationTimelineEntry
-  init(date:complicationTemplate:) Deprecated

Initializer

# init(date:complicationTemplate:)

Creates and returns a timeline entry with the specified date and complication data.

watchOS 2.0–9.0Deprecated

``` source
convenience init(
    date: Date,
    complicationTemplate: CLKComplicationTemplate
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`date`  

The time at which to display the complication data.

`complicationTemplate`  

The complication template containing the data to display. The template must belong to the family of the associated complication.

## Return Value

A timeline entry initialized with the specified data.

## Discussion

Use this method to create new timeline entries. You can change the values of the timeline entry later by modifying the properties of the returned object. This method sets the value of the timelineAnimationGroup property to `nil`.

## See Also

### Creating a Timeline Entry

convenience init(date: Date, complicationTemplate: CLKComplicationTemplate, timelineAnimationGroup: String?)

Creates and returns a timeline entry with the specified information.

Deprecated

