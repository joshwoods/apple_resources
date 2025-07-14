

- Core Services
- Apple Events
-  AEStreamOpenEvent(\_:) 

Function

# AEStreamOpenEvent(\_:)

Opens a stream for an existing Apple event.

macOS 10.0+

``` source
func AEStreamOpenEvent(_ event: UnsafeMutablePointer!) -> AEStreamRef!
```

## Parameters 

`event`  

An existing Apple event. See AppleEvent.

## Return Value

An AEStreamRef for the Apple event or `NULL` if the stream data structures could not be allocated.

## Discussion

Use this function to open a stream and add parameters to an existing Apple event. This function copies any parameters already in the Apple event to the stream prior to returning the `AEStreamRef`. When you are done adding parameters, use AEStreamClose(_:_:) to save them to the Apple event and close the stream.

If there is not enough available storage to complete the operation, `AEStreamOpenEvent` returns `NULL` and leaves the Apple event unchanged.

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

