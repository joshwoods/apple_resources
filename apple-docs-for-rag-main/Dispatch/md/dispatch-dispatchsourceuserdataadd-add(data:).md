

- Dispatch
- DispatchSourceUserDataAdd
-  add(data:) 

Instance Method

# add(data:)

Adds the value to the current pending data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func add(data: UInt)
```

## Parameters 

`data`  

The value you want to add the dispatch source.

## Discussion

After you call this method, the dispatch source submits its event handler to its target queue to process the data. If you specify `0` for the data parameter, the dispatch source does not submit its event hander for execution.

