

- Foundation
- NSAppleEventDescriptor
-  transactionID 

Instance Property

# transactionID

The receiver’s transaction ID, if any.

Mac Catalyst 13.0+macOS 10.0+

``` source
var transactionID: AETransactionID { get }
```

## Discussion

The receiver’s transaction ID (an integer value), or 0 if an error occurs.

The receiver must be an Apple event. Currently provides no indication if an error occurs. For more information on transactions, see the description for appleEvent(withEventClass:eventID:targetDescriptor:returnID:transactionID:).

## See Also

### Working With Apple Event Descriptors

func attributeDescriptor(forKeyword: AEKeyword) -> NSAppleEventDescriptor?

Returns a descriptor for the receiver’s Apple event attribute identified by the specified keyword.

var eventClass: AEEventClass

The event class for the receiver.

var eventID: AEEventID

The event ID for the receiver.

func paramDescriptor(forKeyword: AEKeyword) -> NSAppleEventDescriptor?

Returns a descriptor for the receiver’s Apple event parameter identified by the specified keyword.

func removeParamDescriptor(withKeyword: AEKeyword)

Removes the receiver’s parameter descriptor identified by the specified keyword.

var returnID: AEReturnID

The receiver’s return ID (the ID for a reply Apple event).

func setAttribute(NSAppleEventDescriptor, forKeyword: AEKeyword)

Adds a descriptor to the receiver as an attribute identified by the specified keyword.

func setParam(NSAppleEventDescriptor, forKeyword: AEKeyword)

Adds a descriptor to the receiver as an Apple event parameter identified by the specified keyword.

