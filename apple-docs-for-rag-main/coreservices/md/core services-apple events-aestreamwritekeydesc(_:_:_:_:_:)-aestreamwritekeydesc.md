

- Core Services
- Apple Events
-  AEStreamWriteKeyDesc(\_:\_:\_:\_:\_:) 

Function

# AEStreamWriteKeyDesc(\_:\_:\_:\_:\_:)

Writes a complete keyword/descriptor pair to an `AEStreamRef`.

macOS 10.0+

``` source
func AEStreamWriteKeyDesc(
    _ ref: AEStreamRef!,
    _ key: AEKeyword,
    _ newType: DescType,
    _ data: UnsafeRawPointer!,
    _ length: Size
) -> OSStatus
```

## Parameters 

`ref`  

An AEStreamRef containing the stream data.

`key`  

The `AEKeyword` associated with the new descriptor being added to the stream. See AEKeyword.

`newType`  

A type code for the new `AEDesc` being added to the stream. See DescType.

`data`  

A pointer to the block of memory containing the descriptor data. This routine copies the memory block immediately, so you do not need to retain it for the benefit of this routine.

`length`  

The number of bytes pointed to by the `data` parameter.

## Return Value

A result code. See Result Codes.

## Discussion

Use this routine to add a descriptor to the currently open `AERecord` inside a stream. You cannot use this routine to write parameters to any other types of descriptors, even if they are nested inside of an `AERecord`. This routine can only be called in between calls to AEStreamOpenRecord(_:_:) and AEStreamCloseRecord(_:).

This method is analogous to the Apple Event Manager routine AEPutParamPtr(_:_:_:_:_:), except it is for use with streams.

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

func AEStreamCreateEvent(AEEventClass, AEEventID, DescType, UnsafeRawPointer!, Size, Int16, Int32) -> AEStreamRef!

Creates a new Apple event and opens a stream for writing data to it.

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

