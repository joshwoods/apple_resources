

- Dispatch
- DispatchQoS
-  init(qosClass:relativePriority:) 

Initializer

# init(qosClass:relativePriority:)

Creates a new `DispatchQoS` object with the specified QoS class and relative priority.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    qosClass: DispatchQoS.QoSClass,
    relativePriority: Int
)
```

## Parameters 

`qosClass`  

The QoS class.

For possible values, see DispatchQoS.QoSClass.

`relativePriority`  

The relative priority.

## See Also

### Creating a QoS Structure

enum QoSClass

Quality-of-service classes that specify the priorities for executing tasks.

