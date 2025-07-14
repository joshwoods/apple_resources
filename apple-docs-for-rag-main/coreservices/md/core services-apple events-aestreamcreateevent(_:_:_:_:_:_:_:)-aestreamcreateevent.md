

- Core Services
- Apple Events
-  AEStreamCreateEvent(\_:\_:\_:\_:\_:\_:\_:) 

Function

# AEStreamCreateEvent(\_:\_:\_:\_:\_:\_:\_:)

Creates a new Apple event and opens a stream for writing data to it.

macOS 10.0+

``` source
func AEStreamCreateEvent(
    _ clazz: AEEventClass,
    _ id: AEEventID,
    _ targetType: DescType,
    _ targetData: UnsafeRawPointer!,
    _ targetLength: Size,
    _ returnID: Int16,
    _ transactionID: Int32
) -> AEStreamRef!
```

## Parameters 

`clazz`  

The event class of the Apple event. See AEEventClass.

`id`  

The event ID of the Apple event. See AEEventID.

`targetType`  

The address type for the addressing information in the next two parameters. Usually contains one of the following values: `typeApplSignature`. `typeKernelProcessID`, or `typeProcessSerialNumber`. See DescType.

`targetData`  

A pointer to the address information. The data in this pointer must match the data associated with the specified `targetType`.

`targetLength`  

The number of bytes pointed to by the `targetData` parameter.

`returnID`  

The return ID for the created Apple event. If you pass a value of `kAutoGenerateReturnID`, the Apple Event Manager assigns the created Apple event a return ID that is unique to the current session. If you pass any other value, the Apple Event Manager assigns that value for the ID. The return ID constant is described in ID Constants for the AECreateAppleEvent Function. See AEReturnID.

`transactionID`  

The transaction ID for this Apple event. A transaction is a sequence of Apple events that are sent back and forth between the client and server applications, beginning with the client’s initial request for a service. All Apple events that are part of a transaction must have the same transaction ID. You can specify the `kAnyTransactionID` constant if the Apple event is not one of a series of interdependent Apple events. This transaction ID constant is described in ID Constants for the AECreateAppleEvent Function. See AETransactionID.

## Return Value

An AEStreamRef associated with the new event.

## Discussion

This routine effectively combines a call to AECreateAppleEvent(_:_:_:_:_:_:) followed by a call to AEStreamOpenEvent(_:) to create a new Apple event in the stream. You can use the returned `AEStreamRef` to add parameters to the new Apple event.

## See Also

### Creating Apple Event Structures Using Streams

func AEStreamClose(AEStreamRef!, UnsafeMutablePointer&lt;AEDesc>!) -> OSStatus

Closes and deallocates an `AEStreamRef`.

func AEStreamCloseDesc(AEStreamRef!) -> OSStatus

Marks the end of a descriptor in an `AEStreamRef`.

func AEStreamCloseList(AEStreamRef!) -> OSStatus

Marks the end of a list of descriptors in an `AEStreamRef`.

func AEStreamCloseRecord(AEStreamRef!) -> OSStatus

Marks the end of a record in an `AEStreamRef`.

func AEStreamOpen() -> AEStreamRef!

Opens a new `AEStreamRef` for use in building a descriptor.

func AEStreamOpenDesc(AEStreamRef!, DescType) -> OSStatus

Marks the beginning of a descriptor in an `AEStreamRef`.

func AEStreamOpenEvent(UnsafeMutablePointer&lt;AppleEvent>!) -> AEStreamRef!

Opens a stream for an existing Apple event.

func AEStreamOpenKeyDesc(AEStreamRef!, AEKeyword, DescType) -> OSStatus

Marks the beginning of a key descriptor in an `AEStreamRef`.

func AEStreamOpenList(AEStreamRef!) -> OSStatus

Marks the beginning of a descriptor list in an `AEStreamRef`.

func AEStreamOpenRecord(AEStreamRef!, DescType) -> OSStatus

Marks the beginning of an Apple event record in an `AEStreamRef`.

func AEStreamOptionalParam(AEStreamRef!, AEKeyword) -> OSStatus

Designates a parameter in an Apple event as optional.

func AEStreamSetRecordType(AEStreamRef!, DescType) -> OSStatus

Sets the type of the most recently created record in an `AEStreamRef`.

func AEStreamWriteAEDesc(AEStreamRef!, UnsafePointer&lt;AEDesc>!) -> OSStatus

Copies an existing descriptor into an `AEStreamRef`.

func AEStreamWriteData(AEStreamRef!, UnsafeRawPointer!, Size) -> OSStatus

Appends data to the current descriptor in an `AEStreamRef`.

func AEStreamWriteDesc(AEStreamRef!, DescType, UnsafeRawPointer!, Size) -> OSStatus

Appends the data for a complete descriptor to an `AEStreamRef`.

func AEStreamWriteKey(AEStreamRef!, AEKeyword) -> OSStatus

Marks the beginning of a keyword/descriptor pair for a descriptor in an `AEStreamRef`.

func AEStreamWriteKeyDesc(AEStreamRef!, AEKeyword, DescType, UnsafeRawPointer!, Size) -> OSStatus

Writes a complete keyword/descriptor pair to an `AEStreamRef`.

