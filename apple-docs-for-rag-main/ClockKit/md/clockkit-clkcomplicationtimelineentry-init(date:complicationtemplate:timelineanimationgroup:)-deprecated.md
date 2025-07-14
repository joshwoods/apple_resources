

- ClockKit
- CLKComplicationTimelineEntry
-  init(date:complicationTemplate:timelineAnimationGroup:) Deprecated

Initializer

# init(date:complicationTemplate:timelineAnimationGroup:)

Creates and returns a timeline entry with the specified information.

watchOS 2.0–9.0Deprecated

``` source
convenience init(
    date: Date,
    complicationTemplate: CLKComplicationTemplate,
    timelineAnimationGroup: String?
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`date`  

The time at which to display the complication data.

`complicationTemplate`  

The complication template containing the data to display. Specify a template that’s appropriate for the complication family.

`timelineAnimationGroup`  

The animation group with which to associate the entry. For more information about how this value is used, see timelineAnimationGroup.

## Return Value

A timeline entry initialized with the specified data.

## Discussion

Use this method to create new timeline entries. You can change the values of the timeline entry later by modifying the properties of the returned object.

## See Also

### Creating a Timeline Entry

convenience init(date: Date, complicationTemplate: CLKComplicationTemplate)

Creates and returns a timeline entry with the specified date and complication data.

Deprecated

