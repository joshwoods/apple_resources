

- WidgetKit
- IntentRecommendation
-  init(intent:description:) 

Initializer

# init(intent:description:)

Creates a recommended configuration for a widget on platforms that don’t offer a dedicated user interface to customize widgets with a localized description.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 9.0+

``` source
init(
    intent: T,
    description: LocalizedStringKey
)
```

## Parameters 

`intent`  

The intent that represents the recommended configuration.

`description`  

A key for a localized string in your bundle that helps the user understand the value of the preconfigured configuration option. For example, if the configuration represents a location in a weather app, the description may be the name of one of the user’s favorite cities, such as `Cupertino`.

## Discussion

Note

On platforms that offer a dedicated user interface for configuring widgets — for example, iOS or macOS — `IntentRecommendation` is inactive.

## See Also

### Creating a Recommended Widget Configuration

init(intent: T, description: Text)

Creates a recommended configuration for a widget on platforms that don’t offer a dedicated user interface to customize widgets.

init&lt;S>(intent: T, description: S)

Creates a recommended configuration for a widget on platforms that don’t offer a dedicated user interface to customize widgets.

