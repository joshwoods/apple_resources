

- Foundation
- NSAppleEventDescriptor
-  init(eventClass:eventID:targetDescriptor:returnID:transactionID:) 

Initializer

# init(eventClass:eventID:targetDescriptor:returnID:transactionID:)

Initializes a newly allocated instance as a descriptor for an Apple event, initialized with the specified values.

Mac Catalyst 13.0+macOS 10.0+

``` source
convenience init(
    eventClass: AEEventClass,
    eventID: AEEventID,
    targetDescriptor: NSAppleEventDescriptor?,
    returnID: AEReturnID,
    transactionID: AETransactionID
)
```

## Parameters 

`eventClass`  

The event class to be set in the returned descriptor.

`eventID`  

The event ID to be set in the returned descriptor.

`targetDescriptor`  

A pointer to a descriptor that identifies the target application for the Apple event. Passing `nil` results in an Apple event descriptor that has no `keyAddressAttr` attribute (it is valid for an Apple event to have no target address attribute).

`returnID`  

The return ID to be set in the returned descriptor. If you pass a value of `kAutoGenerateReturnID`, the Apple Event Manager assigns the created Apple event a return ID that is unique to the current session. If you pass any other value, the Apple Event Manager assigns that value for the ID.

`transactionID`  

The transaction ID to be set in the returned descriptor. A transaction is a sequence of Apple events that are sent back and forth between client and server applications, beginning with the client’s initial request for a service. All Apple events that are part of a transaction must have the same transaction ID. You can specify `kAnyTransactionID` if the Apple event is not one of a series of interdependent Apple events.

## Return Value

The initialized Apple event (an instance of `NSAppleEventDescriptor`), or `nil` if an error occurs.

## See Also

### Creating and Initializing Descriptors

class func appleEvent(withEventClass: AEEventClass, eventID: AEEventID, targetDescriptor: NSAppleEventDescriptor?, returnID: AEReturnID, transactionID: AETransactionID) -> NSAppleEventDescriptor

Creates a descriptor that represents an Apple event, initialized according to the specified information.

init(boolean: Bool)

Creates a descriptor initialized with type `typeBoolean` that stores the specified Boolean value.

init(enumCode: OSType)

Creates a descriptor initialized with type `typeEnumerated` that stores the specified enumerator data type value.

init(int32: Int32)

Creates a descriptor initialized with Apple event type `typeSInt32` that stores the specified integer value.

init(string: String)

Creates a descriptor initialized with type `typeUnicodeText` that stores the text from the specified string.

init(typeCode: OSType)

Creates a descriptor initialized with type `typeType` that stores the specified type value.

class func list() -> NSAppleEventDescriptor

Creates and initializes an empty list descriptor.

class func null() -> NSAppleEventDescriptor

Creates and initializes a descriptor with no parameter or attribute values set.

class func record() -> NSAppleEventDescriptor

Creates and initializes a descriptor for an Apple event record whose data has yet to be set.

convenience init(listDescriptor: ())

Initializes a newly allocated instance as an empty list descriptor.

convenience init(recordDescriptor: ())

Initializes a newly allocated instance as a descriptor that is an Apple event record.

init(aeDescNoCopy: UnsafePointer&lt;AEDesc>)

Initializes a newly allocated instance as a descriptor for the specified Carbon `AEDesc` structure.

convenience init?(descriptorType: DescType, bytes: UnsafeRawPointer?, length: Int)

Initializes a newly allocated instance as a descriptor with the specified descriptor type and data (from an arbitrary sequence of bytes and a length count).

convenience init?(descriptorType: DescType, data: Data?)

Initializes a newly allocated instance as a descriptor with the specified descriptor type and data (from an instance of `NSData`).

