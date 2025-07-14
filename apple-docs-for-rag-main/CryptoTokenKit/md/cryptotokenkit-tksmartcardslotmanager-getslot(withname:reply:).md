

- CryptoTokenKit
- TKSmartCardSlotManager
-  getSlot(withName:reply:) 

Instance Method

# getSlot(withName:reply:)

Asynchronously calls a block with a Smart Card reader slot for a specified name.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func getSlot(
    withName name: String,
    reply: @escaping (TKSmartCardSlot?) -> Void
)
```

``` source
func getSlot(withName name: String) async -> TKSmartCardSlot?
```

## Parameters 

`name`  

The name of the Smart Card reader slot.

`reply`  

slot  
The Smart Card reader slot corresponding to the specified name. If no slot exists with that name, this argument is `nil`.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func getSlot(withName name: String) async -> TKSmartCardSlot?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Accessing Smart Card Slots

var slotNames: [String]

A list of identifiers for all the Smart Card reader slots available to the system.

func slotNamed(String) -> TKSmartCardSlot?

Returns the Smart Card slot with a given name.

