

- Core Services
- Apple Events
-  AEStreamClose(\_:\_:) 

Function

# AEStreamClose(\_:\_:)

Closes and deallocates an `AEStreamRef`.

macOS 10.0+

``` source
func AEStreamClose(
    _ ref: AEStreamRef!,
    _ desc: UnsafeMutablePointer!
) -> OSStatus
```

## Parameters 

`ref`  

An AEStreamRefcontaining the stream data.

`desc`  

A pointer to a descriptor for receiving a the stream data, or `NULL` if you want to discard the data. See AEDesc.

## Return Value

A result code. See Result Codes.

## Discussion

Use this function to dispose of an `AEStreamRef` you created using AEStreamCreateEvent(_:_:_:_:_:_:_:), AEStreamOpen(), or AEStreamOpenEvent(_:). To retrieve the resulting descriptor from the stream prior to disposal, pass in a pointer to an `AEDesc` structure in the `desc` parameter. If this parameter exists, `AEStreamClose` fills in the descriptor with the stream data. If the stream contains invalid information, possibly due to improperly balanced calls to “AEStream” functions, the returned descriptor type is set to `typeNull`.

Regardless of any errors returned by this function, it is always safe to call AEDisposeDesc(_:) on the returned descriptor.

Specifying `NULL` for the `desc` parameter causes `AEStreamClose` to discard the stream data and dispose of the `AEStreamRef`. When you call `AEStreamClose` in this way, you do not need to worry about balancing nested calls to “AEStream” functions. This technique is particularly useful during error-handling situations where you need to dispose of a stream but do not know its exact state.

## See Also

### Creating Apple Event Structures Using Streams

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

func AEStreamWriteKeyDesc(AEStreamRef!, AEKeyword, DescType, UnsafeRawPointer!, Size) -> OSStatus

Writes a complete keyword/descriptor pair to an `AEStreamRef`.

