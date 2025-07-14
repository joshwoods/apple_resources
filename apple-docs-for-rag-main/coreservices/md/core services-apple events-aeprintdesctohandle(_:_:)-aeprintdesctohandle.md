

- Core Services
- Apple Events
-  AEPrintDescToHandle(\_:\_:) 

Function

# AEPrintDescToHandle(\_:\_:)

Provides a pretty printer facility for displaying the contents of Apple event descriptors.

macOS 10.0+

``` source
func AEPrintDescToHandle(
    _ desc: UnsafePointer!,
    _ result: UnsafeMutablePointer!
) -> OSStatus
```

## Parameters 

`desc`  

A pointer to a descriptor containing the information to be printed. See AEDesc.

`result`  

A pointer to a location for a new `Handle` data type. On return, contains a new handle allocated by the Memory Manager.

## Return Value

A result code. See Result Codes.

## Discussion

The data handle returned in the `result` parameter contains a text string formatted using the “AEBuild” syntax. This string is useful for looking at the contents of Apple events sent by other applications and for debugging your own descriptors.

`AEPrintDescToHandle` prints the contents of `AEDesc`, `AERecord`, and `AEDescList` descriptors in a format that is suitable for input to AEBuildDesc. `AEPrintDescToHandle` also attempts display coerced Apple event records as the coerced record type instead of as the original type. Any data structures that cannot be identified are displayed as hexadecimal data.

`AEPrintDescToHandle` prints the contents of Apple events in a slightly different format. For these events, the event class and event ID appear at the beginning of the output string, followed by the contents of the event enclosed in curly braces. In addition, each attribute is printed with its four-character identifier and preceded by an ampersand character. You cannot use the output string to recreate the Apple event from AEBuildAppleEvent.

## See Also

### Creating Apple Event Structures in Memory

func vAEBuildAppleEvent(AEEventClass, AEEventID, DescType, UnsafeRawPointer!, Size, Int16, Int32, UnsafeMutablePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AEBuildError>!, UnsafePointer&lt;CChar>!, CVaListPointer) -> OSStatus

Allows you to encapsulate calls to `AEBuildAppleEvent` in a wrapper routine.

func vAEBuildDesc(UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEBuildError>!, UnsafePointer&lt;CChar>!, CVaListPointer) -> OSStatus

Allows you to encapsulate calls to `AEBuildDesc` in your own wrapper routines.

func vAEBuildParameters(UnsafeMutablePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AEBuildError>!, UnsafePointer&lt;CChar>!, CVaListPointer) -> OSStatus

Allows you to encapsulate calls to `AEBuildParameters` in your own `stdarg`-style wrapper routines, using techniques similar to those allowed by vsprintf.

