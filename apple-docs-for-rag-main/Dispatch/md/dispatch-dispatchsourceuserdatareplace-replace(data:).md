

- Dispatch
- DispatchSourceUserDataReplace
-  replace(data:) 

Instance Method

# replace(data:)

Replaces the current pending data with the new value you provide.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func replace(data: UInt)
```

## Parameters 

`data`  

The data that replaces the current pending value.

## Discussion

After you call this method, the dispatch source submits its event handler to its target queue to process the data. If you specify `0` for the data parameter, the dispatch source does not submit its event hander for execution.

