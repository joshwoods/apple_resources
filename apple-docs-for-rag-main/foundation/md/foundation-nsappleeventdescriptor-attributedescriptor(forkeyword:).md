

- Foundation
- NSAppleEventDescriptor
-  attributeDescriptor(forKeyword:) 

Instance Method

# attributeDescriptor(forKeyword:)

Returns a descriptor for the receiver’s Apple event attribute identified by the specified keyword.

Mac Catalyst 13.0+macOS 10.0+

``` source
func attributeDescriptor(forKeyword keyword: AEKeyword) -> NSAppleEventDescriptor?
```

## Parameters 

`keyword`  

A keyword (a four-character code) that identifies the descriptor to obtain.

## Return Value

The attribute descriptor for the specified keyword, or `nil` if an error occurs.

## Discussion

The receiver must be an Apple event.

## See Also

### Working With Apple Event Descriptors

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

var transactionID: AETransactionID

The receiver’s transaction ID, if any.

