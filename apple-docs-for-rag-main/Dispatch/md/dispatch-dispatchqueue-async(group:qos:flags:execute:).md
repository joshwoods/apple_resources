

- Dispatch
- DispatchQueue
-  async(group:qos:flags:execute:) 

Instance Method

# async(group:qos:flags:execute:)

Schedules a block asynchronously for execution and optionally associates it with a dispatch group.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
@preconcurrency
func async(
    group: DispatchGroup? = nil,
    qos: DispatchQoS = .unspecified,
    flags: DispatchWorkItemFlags = [],
    execute work: @escaping () -> Void
)
```

## Parameters 

`group`  

The dispatch group to associate with the work item. If you specify `NULL`, the block is not associated with a group.

`qos`  

The quality-of-service class to use when executing the block. This parameter determines the priority with which the block is scheduled and executed. For a list of possible values, see DispatchQoS.

`flags`  

Additional attributes to apply when executing the block. For a list of possible values, see DispatchWorkItemFlags.

`work`  

The block containing the work to perform. This block has no return value and no parameters.

## See Also

### Dispatching Work to Groups

func async(group: DispatchGroup, execute: DispatchWorkItem)

Schedules a work item asynchronously for execution and associates it with the specified dispatch group.

