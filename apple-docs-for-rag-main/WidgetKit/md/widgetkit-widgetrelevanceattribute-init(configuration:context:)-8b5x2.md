

- WidgetKit
- WidgetRelevanceAttribute
-  init(configuration:context:) 

Initializer

# init(configuration:context:)

Creates a new widget relevance for a specific configuration that is relevant in a specific context.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
init(
    configuration: Configuration,
    context: RelevantContext
)
```

Available when `Configuration` inherits `INIntent`.

## Parameters 

`configuration`  

The specific configuration

`context`  

The relevant context where this widget is relevant.

## Discussion

For example, a weather widget could specify that a configuration for a specific location is relevant for a the relevant context at that specific location.

