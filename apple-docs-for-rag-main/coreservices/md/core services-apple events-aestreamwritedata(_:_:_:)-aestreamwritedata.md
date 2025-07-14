

- Core Services
- Apple Events
-  AEStreamWriteData(\_:\_:\_:) 

Function

# AEStreamWriteData(\_:\_:\_:)

Appends data to the current descriptor in an `AEStreamRef`.

macOS 10.0+

``` source
func AEStreamWriteData(
    _ ref: AEStreamRef!,
    _ data: UnsafeRawPointer!,
    _ length: Size
) -> OSStatus
```

## Parameters 

`ref`  

An AEStreamRef containing the stream data.

`data`  

A pointer to the block of memory containing the descriptor data. This routine copies the memory block immediately, so you do not need to retain it for the benefit of this routine.

`length`  

The number of bytes pointed to by the `data` parameter.

## Return Value

A result code. See Result Codes.

## Discussion

You can call this routine any number of times to build up the data contents of the descriptor incrementally. You must precede calls to this routine by a call to either AEStreamOpenDesc(_:_:) or AEStreamOpenKeyDesc(_:_:_:). When you are done adding data to the descriptor, call AEStreamCloseDesc(_:) to complete the descriptor definition.

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

func AEStreamWriteDesc(AEStreamRef!, DescType, UnsafeRawPointer!, Size) -> OSStatus

Appends the data for a complete descriptor to an `AEStreamRef`.

func AEStreamWriteKey(AEStreamRef!, AEKeyword) -> OSStatus

Marks the beginning of a keyword/descriptor pair for a descriptor in an `AEStreamRef`.

func AEStreamWriteKeyDesc(AEStreamRef!, AEKeyword, DescType, UnsafeRawPointer!, Size) -> OSStatus

Writes a complete keyword/descriptor pair to an `AEStreamRef`.

