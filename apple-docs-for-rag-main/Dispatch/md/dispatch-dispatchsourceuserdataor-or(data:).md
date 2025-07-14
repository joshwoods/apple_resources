

- Dispatch
- DispatchSourceUserDataOr
-  or(data:) 

Instance Method

# or(data:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func or(data: UInt)
```

## Parameters 

`data`  

The value you want to merge with the existing data in the dispatch source. The dispatch source ORs this value with the currently pending data.

## Discussion

After you call this method, the dispatch source submits its event handler to its target queue to process the data. If you specify `0` for the data parameter, the dispatch source does not submit its event hander for execution.

