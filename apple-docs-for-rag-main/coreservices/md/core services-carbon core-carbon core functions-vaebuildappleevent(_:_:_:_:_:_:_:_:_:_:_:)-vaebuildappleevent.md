

- Core Services
- Carbon Core
- Carbon Core Functions
-  vAEBuildAppleEvent(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# vAEBuildAppleEvent(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Allows you to encapsulate calls to `AEBuildAppleEvent` in a wrapper routine.

macOS 10.0+

``` source
func vAEBuildAppleEvent(
    _ theClass: AEEventClass,
    _ theID: AEEventID,
    _ addressType: DescType,
    _ addressData: UnsafeRawPointer!,
    _ addressLength: Size,
    _ returnID: Int16,
    _ transactionID: Int32,
    _ resultEvt: UnsafeMutablePointer!,
    _ error: UnsafeMutablePointer!,
    _ paramsFmt: UnsafePointer!,
    _ args: CVaListPointer
) -> OSStatus
```

## Parameters 

`theClass`  

The event class for the resulting Apple event. See AEEventClass.

`theID`  

The event id for the resulting Apple event. See AEEventID.

`addressType`  

The address type for the addressing information described in the next two parameters: usually one of `typeApplSignature`, `typeProcessSerialNumber`, or `typeKernelProcessID`. See DescType.

`addressData`  

A pointer to the address information.

`addressLength`  

The number of bytes pointed to by the `addressData` parameter.

`returnID`  

The return ID for the created Apple event. If you pass a value of `kAutoGenerateReturnID`, the Apple Event Manager assigns the created Apple event a return ID that is unique to the current session. If you pass any other value, the Apple Event Manager assigns that value for the ID.

`transactionID`  

The transaction ID for this Apple event. A transaction is a sequence of Apple events that are sent back and forth between the client and server applications, beginning with the client’s initial request for a service. All Apple events that are part of a transaction must have the same transaction ID. You can specify the `kAnyTransactionID` constant if the Apple event is not one of a series of interdependent Apple events.

`result`  

A pointer to a descriptor where the resulting descriptor should be stored. See AppleEvent for a description of the data type.

`error`  

A pointer to an `AEBuildError` structure where additional information about any errors that occur will be saved. This is an optional parameter and you can pass `NULL` if this information is not required. See AEBuildErrorCode for the syntax error codes that can be returned in this structure.

`paramsFmt`  

An AEBuild format string describing the AppleEvent record to be created. The format of these strings is described in Technical Note TN2106, AEBuild*, AEPrint*, and Friends.

`args`  

A variable array of arguments to be substituted into the `paramsFmt` format string. See the ANSI C Interfaces documentation for a description of the `va_list` data type.

## Return Value

A result code. See Result Codes.

## Discussion

Passing an argument list to `vAEBuildAppleEvent` corresponds to passing a series of individual parameters to the AEBuildAppleEvent function.

This function and related “AEBuild” routines provide a very simple translation service for converting specially formatted strings into complex Apple event descriptors. Normally, creating complex Apple event descriptors requires a large number of calls to Apple event Manager routines to build up the descriptor piece by piece. The `vAEBuildAppleEvent` function and related routines allow you to consolidate all of the calls required to construct a complex Apple event descriptor into a single system call that creates the desired structure as directed by a format string that you provide.

## See Also

### Creating Apple Event Structures in Memory

func AEPrintDescToHandle(UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;Handle?>!) -> OSStatus

Provides a pretty printer facility for displaying the contents of Apple event descriptors.

func vAEBuildDesc(UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEBuildError>!, UnsafePointer&lt;CChar>!, CVaListPointer) -> OSStatus

Allows you to encapsulate calls to `AEBuildDesc` in your own wrapper routines.

func vAEBuildParameters(UnsafeMutablePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AEBuildError>!, UnsafePointer&lt;CChar>!, CVaListPointer) -> OSStatus

Allows you to encapsulate calls to `AEBuildParameters` in your own `stdarg`-style wrapper routines, using techniques similar to those allowed by vsprintf.

