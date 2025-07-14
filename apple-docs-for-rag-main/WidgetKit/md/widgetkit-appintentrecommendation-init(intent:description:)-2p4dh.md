

- WidgetKit
- AppIntentRecommendation
-  init(intent:description:) 

Initializer

# init(intent:description:)

Creates a recommended configuration for a widget on platforms that don’t offer a dedicated user interface to customize widgets with a localized description.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+watchOS 10.0+

``` source
init(
    intent: Intent,
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

On platforms that offer a dedicated user interface for configuring widgets — for example, iOS or macOS — `AppIntentRecommendation` is inactive.

## See Also

### Creating a recommended widget configuration

init(intent: Intent, description: Text)

Creates a recommended configuration for a widget on platforms that don’t offer a dedicated user interface to customize widgets.

init(intent: Intent, description: some StringProtocol)

Creates a recommended configuration for a widget on platforms that don’t offer a dedicated user interface to customize widgets.

