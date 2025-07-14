

- Core Services
- Apple Events
-  AEStreamWriteKey(\_:\_:) 

Function

# AEStreamWriteKey(\_:\_:)

Marks the beginning of a keyword/descriptor pair for a descriptor in an `AEStreamRef`.

macOS 10.0+

``` source
func AEStreamWriteKey(
    _ ref: AEStreamRef!,
    _ key: AEKeyword
) -> OSStatus
```

## Parameters 

`ref`  

An AEStreamRef containing the stream data.

`key`  

The `AEKeyword` associated with the new descriptor being added to the stream. See AEKeyword.

## Return Value

A result code. See Result Codes.

## Discussion

You must follow this call with a sequence of “AEStream” calls to specify exactly one descriptor that goes with the keyword. The descriptor you create can be of type `AEDesc`, `AEDescList`, or `AERecord`.

If you are creating nested descriptors, this routine begins a new keyword/descriptor pair for the descriptor most recently opened by a call to AEStreamWriteKey(_:_:) or AEStreamOpenEvent(_:). You cannot use this routine to write parameters to any other types of descriptors, even if they are nested inside of an `AERecord`.

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

func AEStreamWriteKeyDesc(AEStreamRef!, AEKeyword, DescType, UnsafeRawPointer!, Size) -> OSStatus

Writes a complete keyword/descriptor pair to an `AEStreamRef`.

