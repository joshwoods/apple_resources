

- ClockKit
- CLKComplicationDescriptor
-  init(identifier:displayName:supportedFamilies:) Deprecated

Initializer

# init(identifier:displayName:supportedFamilies:)

Returns a new complication descriptor.

watchOS 7.0–9.0Deprecated

``` source
convenience init(
    identifier: String,
    displayName: String,
    supportedFamilies: [CLKComplicationFamily]
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`identifier`  

A string that uniquely identifies the descriptor.

`displayName`  

A localized name that ClockKit shows to the user to identify complications from the descriptor.

`supportedFamilies`  

The families that support this type of complication. Note that different descriptors can support different sets of families.

## See Also

### Creating descriptors

convenience init(identifier: String, displayName: String, supportedFamilies: [CLKComplicationFamily], userActivity: NSUserActivity)

Returns a new complication descriptor with an associated user activity.

Deprecated

convenience init(identifier: String, displayName: String, supportedFamilies: [CLKComplicationFamily], userInfo: [AnyHashable : Any])

Returns a new complication descriptor with an associated dictionary of user data.

Deprecated

