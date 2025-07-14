

- WidgetKit
- WidgetCenter
-  invalidateConfigurationRecommendations() 

Instance Method

# invalidateConfigurationRecommendations()

Invalidates and refreshes the preconfigured intent configurations for user-customizable widgets.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 9.0+

``` source
func invalidateConfigurationRecommendations()
```

## Mentioned in 

Making a configurable widget

## Discussion

In watchOS, call this function when your app receives new data for preconfigured widgets you’d like to appear in the list of available watch complications.

Note

On platforms that offer a dedicated user interface for configuring widgets — for example, iOS or macOS — `invalidateConfigurationRecommendations()` is inactive.

