

- ClockKit
- CLKComplicationIntentWidgetMigrationConfiguration
-  init(kind:extensionBundleIdentifier:intent:localizedDisplayName:) 

Initializer

# init(kind:extensionBundleIdentifier:intent:localizedDisplayName:)

Creates an object that describes an intents-based watchOS complication in your WidgetKit extension.

watchOS 9.0+

``` source
init(
    kind: String,
    extensionBundleIdentifier: String,
    intent: INIntent,
    localizedDisplayName: String
)
```

## Parameters 

`kind`  

A string that uniquely identifies a widget in your WidgetKit extension.

`extensionBundleIdentifier`  

The bundle identifier for your WidgetKit extension.

`intent`  

A SiriKit intent that provides additional configuration information to your WidgetKit complication.

`localizedDisplayName`  

A localized name for the complication.

