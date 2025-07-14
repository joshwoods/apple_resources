

- Dispatch
- DispatchSource
-  makeUserDataAddSource(queue:) 

Type Method

# makeUserDataAddSource(queue:)

Creates a new dispatch source object that you use to coalesce custom app data using an AND operator.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func makeUserDataAddSource(queue: DispatchQueue? = nil) -> any DispatchSourceUserDataAdd
```

## Parameters 

`queue`  

The dispatch queue to use when executing the installed handlers.

## Return Value

A dispatch source object that conforms to the DispatchSourceUserDataAdd protocol.

## Discussion

After creating the dispatch source, use the methods of the DispatchSourceProtocol protocol to install the event handlers you need. The returned dispatch source is in the inactive state initially. When you are ready to begin processing events, call its activate() method.

## See Also

### Creating a Custom Source

class func makeUserDataOrSource(queue: DispatchQueue?) -> any DispatchSourceUserDataOr

Creates a new dispatch source object that you use to coalesce custom app data using an OR operator.

class func makeUserDataReplaceSource(queue: DispatchQueue?) -> any DispatchSourceUserDataReplace

Creates a new dispatch source object that you use to track custom app data.

protocol DispatchSourceUserDataAdd

A dispatch source that coalesces data you provide using an AND operation.

protocol DispatchSourceUserDataOr

A dispatch source that coalesces data you provide using an OR operation.

protocol DispatchSourceUserDataReplace

A dispatch source that replaces any pending data with the new value you provide.

