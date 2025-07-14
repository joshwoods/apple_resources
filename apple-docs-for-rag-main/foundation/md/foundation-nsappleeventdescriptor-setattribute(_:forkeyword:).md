

- Foundation
- NSAppleEventDescriptor
-  setAttribute(\_:forKeyword:) 

Instance Method

# setAttribute(\_:forKeyword:)

Adds a descriptor to the receiver as an attribute identified by the specified keyword.

Mac Catalyst 13.0+macOS 10.0+

``` source
func setAttribute(
    _ descriptor: NSAppleEventDescriptor,
    forKeyword keyword: AEKeyword
)
```

## Parameters 

`descriptor`  

The attribute descriptor to add to the receiver.

`keyword`  

A keyword (a four-character code) that identifies the attribute descriptor to add. If a descriptor with that keyword already exists in the receiver, it is replaced.

## Discussion

The receiver must be an Apple event. Currently provides no indication if an error occurs.

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

func setParam(NSAppleEventDescriptor, forKeyword: AEKeyword)

Adds a descriptor to the receiver as an Apple event parameter identified by the specified keyword.

var transactionID: AETransactionID

The receiver’s transaction ID, if any.

