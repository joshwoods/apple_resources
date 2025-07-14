

- Network Extension
- NEFilterControlProvider
-  handleNewFlow(\_:completionHandler:) 

Instance Method

# handleNewFlow(\_:completionHandler:)

Handle a request for new filtering rules.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func handleNewFlow(
    _ flow: NEFilterFlow,
    completionHandler: @escaping (NEFilterControlVerdict) -> Void
)
```

``` source
func handleNewFlow(_ flow: NEFilterFlow) async -> NEFilterControlVerdict
```

## Parameters 

`flow`  

A `NEFilterFlow` object containing details about the flow of network content.

`completionHandler`  

A block to be executed when the rules have been updated.

## Discussion

The system calls this method when the Filter Data Provider indicates that it needs more rules before making a decision about a new flow.

The Filter Control Provider is expected to fetch new rules and write them to disk in a location that is readable by the Filter Data Provider. In addition to updating the rules, the Filter Control Provider can itself make a pass/block decision for the new flow, and return it when executing the `completionHandler` block.

NEFilterControlProvider subclasses must override this method.

## See Also

### Handling requests for new rules

func notifyRulesChanged()

Notify the Filter Data Provider that the filtering rules have changed on disk.

