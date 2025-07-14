

- Core Services
- Apple Events
-  AEStreamOpenKeyDesc(\_:\_:\_:) 

Function

# AEStreamOpenKeyDesc(\_:\_:\_:)

Marks the beginning of a key descriptor in an `AEStreamRef`.

macOS 10.0+

``` source
func AEStreamOpenKeyDesc(
    _ ref: AEStreamRef!,
    _ key: AEKeyword,
    _ newType: DescType
) -> OSStatus
```

## Parameters 

`ref`  

An AEStreamRef containing the stream data.

`key`  

The `AEKeyword` associated with the new descriptor being added to the stream. See AEKeyword.

`newType`  

A type code for the new `AEDesc` being added to the stream. See DescType.

## Return Value

A result code. See Result Codes.

## Discussion

Use this routine to mark the beginning of a keyword/descriptor definition in an Apple event record. After calling this routine, you should call AEStreamWriteData(_:_:_:) one or more times to write the record data to the stream. When you are done writing data, you must call AEStreamCloseDesc(_:) to complete the record definition.

This routine must be called only as part of an Apple event record definition. You cannot use this routine to write keyword/descriptor definitions to other descriptor types, such as an `AEDesc` or `AEDescList`, even if those types are nested inside an Apple event record. In situations where you need to create nested records, this routine opens a new keyword/descriptor definition in the Apple event record associated with the most recent call to AEStreamOpenRecord(_:_:).

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

