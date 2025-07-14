

- ClockKit
- CLKComplication
-  family Deprecated

Instance Property

# family

The family to which the complication belongs.

watchOS 2.0–9.0Deprecated

``` source
var family: CLKComplicationFamily { get }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Mentioned in 

Creating a timeline entry

## Discussion

The family property determines how much space is available to a complication and which templates you can use to display your complication data. In your complication data source, you typically use the property’s value in a `switch` statement when determining the complication template your data source creates.

In watchOS 7 and later, ClockKit represents complications using its family and identifier. Each pair represents a unique complication that the user can select.

In watchOS 6 and earlier, ClockKit represents a complication by its family only. Each family can only have one complication. For more information, see Declaring complications for your app.

## See Also

### Accessing Data About the Complication

var identifier: String

An identifier that specifies a complication if your app supports multiple complications per family.

Deprecated

var userActivity: NSUserActivity?

An object that represents the state of the app at a moment in time.

Deprecated

var userInfo: [AnyHashable : Any]?

A dictionary of additional data associated with the complication.

Deprecated

