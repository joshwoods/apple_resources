

- Dispatch
- DispatchSource
-  makeSignalSource(signal:queue:) 

Type Method

# makeSignalSource(signal:queue:)

Creates a new dispatch source object that monitors the arrival of a UNIX signal.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func makeSignalSource(
    signal: Int32,
    queue: DispatchQueue? = nil
) -> any DispatchSourceSignal
```

## Parameters 

`signal`  

The Unix signal number to monitor.

`queue`  

The dispatch queue to use when executing the installed handlers.

## Return Value

A dispatch source object that conforms to the DispatchSourceSignal protocol.

## Discussion

After creating the dispatch source, use the methods of the DispatchSourceProtocol protocol to install the event handlers you need. The returned dispatch source is in the inactive state initially. When you are ready to begin processing events, call its activate() method.

## See Also

### Creating a Signal Source

protocol DispatchSourceSignal

A dispatch source that monitors the current process for UNIX signals.

