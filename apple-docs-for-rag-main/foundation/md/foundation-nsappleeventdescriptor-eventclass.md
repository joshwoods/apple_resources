

- Foundation
- NSAppleEventDescriptor
-  eventClass 

Instance Property

# eventClass

The event class for the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var eventClass: AEEventClass { get }
```

## Discussion

The event class (a four-character code) for the receiver, or 0 if an error occurs.

The receiver must be an Apple event. An Apple event is identified by its event class and event ID, a pair of four-character codes stored as 32-bit integers. For example, most events in the Standard suite have the four-character code `'core'` (defined as the constant `kAECoreSuite` in `AE.framework`, a subframework of `ApplicationServices.framework`). For more information on event classes and event IDs, see Building an Apple Event in Apple Events Programming Guide.

## See Also

### Working With Apple Event Descriptors

func attributeDescriptor(forKeyword: AEKeyword) -> NSAppleEventDescriptor?

Returns a descriptor for the receiver’s Apple event attribute identified by the specified keyword.

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

