

- Core Services
- Carbon Core
- Carbon Core Functions
-  vAEBuildDesc(\_:\_:\_:\_:) 

Function

# vAEBuildDesc(\_:\_:\_:\_:)

Allows you to encapsulate calls to `AEBuildDesc` in your own wrapper routines.

macOS 10.0+

``` source
func vAEBuildDesc(
    _ dst: UnsafeMutablePointer!,
    _ error: UnsafeMutablePointer!,
    _ src: UnsafePointer!,
    _ args: CVaListPointer
) -> OSStatus
```

## Parameters 

`dst`  

A pointer to a descriptor where the resulting descriptor should be stored. See AEDesc.

`error`  

A pointer to an `AEBuildError` structure where additional information about any errors that occur will be saved. This is an optional parameter and you can pass `NULL` if this information is not required. See AEBuildError.

`src`  

An `AEBuild` format string describing the descriptor to be created.

`args`  

A reference to a previously defined, variable argument parameter list to use with the descriptor-string. The file `` defines macros for declaring and using the `va_list` data type.

## Return Value

A numeric result code indicating the success of the call. A value of `AEBuildSyntaxNoErr` (zero) means the call succeeded. You can use the `error` parameter to discover information about other errors. See Result Codes.

## Discussion

Passing an argument list to `vAEBuildDesc` corresponds to passing a series of individual parameters to the AEBuildDesc function.

This function and related “AEBuild” routines provide a very simple translation service for converting specially formatted strings into complex Apple event descriptors. Normally, creating complex Apple event descriptors requires a large number of calls to Apple Event Manager routines to build up the descriptor piece by piece. The `vAEBuildDesc` function and related routines allow you to consolidate all of the calls required to construct a complex Apple event descriptor into a single system call that creates the desired structure as directed by a format string that you provide.

## See Also

### Creating Apple Event Structures in Memory

func AEPrintDescToHandle(UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;Handle?>!) -> OSStatus

Provides a pretty printer facility for displaying the contents of Apple event descriptors.

func vAEBuildAppleEvent(AEEventClass, AEEventID, DescType, UnsafeRawPointer!, Size, Int16, Int32, UnsafeMutablePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AEBuildError>!, UnsafePointer&lt;CChar>!, CVaListPointer) -> OSStatus

Allows you to encapsulate calls to `AEBuildAppleEvent` in a wrapper routine.

func vAEBuildParameters(UnsafeMutablePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AEBuildError>!, UnsafePointer&lt;CChar>!, CVaListPointer) -> OSStatus

Allows you to encapsulate calls to `AEBuildParameters` in your own `stdarg`-style wrapper routines, using techniques similar to those allowed by vsprintf.

