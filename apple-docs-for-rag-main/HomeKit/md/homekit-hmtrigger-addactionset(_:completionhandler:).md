

- HomeKit
- HMTrigger
-  addActionSet(\_:completionHandler:) 

Instance Method

# addActionSet(\_:completionHandler:)

Adds an action set to the trigger.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func addActionSet(
    _ actionSet: HMActionSet,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func addActionSet(_ actionSet: HMActionSet) async throws
```

## Parameters 

`actionSet`  

The new action set.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## See Also

### Managing Action Sets

var actionSets: [HMActionSet]

Array of all action sets that will be executed by the trigger.

func removeActionSet(HMActionSet, completionHandler: ((any Error)?) -> Void)

Removes an action set from the trigger.

