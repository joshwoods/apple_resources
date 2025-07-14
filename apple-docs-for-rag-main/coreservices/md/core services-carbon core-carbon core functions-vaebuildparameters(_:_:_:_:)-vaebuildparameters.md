

- Core Services
- Carbon Core
- Carbon Core Functions
-  vAEBuildParameters(\_:\_:\_:\_:) 

Function

# vAEBuildParameters(\_:\_:\_:\_:)

Allows you to encapsulate calls to `AEBuildParameters` in your own `stdarg`-style wrapper routines, using techniques similar to those allowed by vsprintf.

macOS 10.0+

``` source
func vAEBuildParameters(
    _ event: UnsafeMutablePointer!,
    _ error: UnsafeMutablePointer!,
    _ format: UnsafePointer!,
    _ args: CVaListPointer
) -> OSStatus
```

## Parameters 

`event`  

The Apple event to which you are adding parameters. See AppleEvent.

`error`  

A pointer to an `AEBuildError` structure where additional information about any errors that occur will be saved. This is an optional parameter and you can pass `NULL` if this information is not required. See AEBuildError.

`format`  

An `AEBuild` format string describing the `AEDesc` parameters to be created.

`args`  

A reference to a previously defined, variable argument parameter list to use with the descriptor-string. The file `` defines macros for declaring and using the `va_list` data type.

## Return Value

A result code. See Result Codes.

## Discussion

Passing an argument list to `vAEBuildParameters` corresponds to passing a series of individual parameters to the AEBuildParameters function.

This function and related “AEBuild” routines provide a very simple translation service for converting specially formatted strings into complex Apple event descriptors. Normally, creating complex Apple event descriptors requires a large number of calls to Apple event Manager routines to build up the descriptor piece by piece. The `vAEBuildParameters` function and related routines allow you to consolidate all of the calls required to construct a complex Apple event descriptor into a single system call that creates the desired structure as directed by a format string that you provide.

## See Also

### Creating Apple Event Structures in Memory

func AEPrintDescToHandle(UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;Handle?>!) -> OSStatus

Provides a pretty printer facility for displaying the contents of Apple event descriptors.

func vAEBuildAppleEvent(AEEventClass, AEEventID, DescType, UnsafeRawPointer!, Size, Int16, Int32, UnsafeMutablePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AEBuildError>!, UnsafePointer&lt;CChar>!, CVaListPointer) -> OSStatus

Allows you to encapsulate calls to `AEBuildAppleEvent` in a wrapper routine.

func vAEBuildDesc(UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEBuildError>!, UnsafePointer&lt;CChar>!, CVaListPointer) -> OSStatus

Allows you to encapsulate calls to `AEBuildDesc` in your own wrapper routines.

