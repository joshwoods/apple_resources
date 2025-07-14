

- WidgetKit
- WidgetInfo
-  widgetConfigurationIntent(of:) 

Instance Method

# widgetConfigurationIntent(of:)

Gets the associated App Intent.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+watchOS 10.0+

``` source
func widgetConfigurationIntent(of intentType: Intent.Type = Intent.self) -> Intent? where Intent : WidgetConfigurationIntent
```

## Parameters 

`intentType`  

The expected type for the App Intent.

## Return Value

An App Intent that contains the user-edited values or nil if there is no associated App Intent or the type does not match `intentType`.

## Mentioned in 

Making a configurable widget

