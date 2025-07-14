

- WidgetKit
- ControlInfo
-  configurationIntent(of:) 

Instance Method

# configurationIntent(of:)

Gets the associated App Intent.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
func configurationIntent(of intentType: Intent.Type = Intent.self) -> Intent? where Intent : ControlConfigurationIntent
```

## Parameters 

`intentType`  

The expected type for the App Intent.

## Return Value

An App Intent that contains the user-edited values or nil if there is no associated App Intent or the type does not match `intentType`.

