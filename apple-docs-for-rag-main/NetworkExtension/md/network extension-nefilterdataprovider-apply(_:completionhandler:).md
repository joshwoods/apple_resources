

- Network Extension
- NEFilterDataProvider
-  apply(\_:completionHandler:) 

Instance Method

# apply(\_:completionHandler:)

Applies a set of filtering rules associated with the provider and changes the default filtering action.

macOS 10.15+

``` source
func apply(
    _ settings: NEFilterSettings?,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func apply(_ settings: NEFilterSettings?) async throws
```

## Parameters 

`settings`  

A NEFilterSettings object containing the filter settings to apply to the system. Pass `nil` to revert to the default settings, which are an empty list of rules and a default action of NEFilterAction.filterData.

`completionHandler`  

A Swift closure or ObjectiveC block that executes when the system finishes applying the settings. It receives an NSError parameter; a non-`nil` value that indicates there’s an error contidition.

## See Also

### Changing filter settings

class NEFilterSettings

The rules and other settings that define the operation of a filter.

