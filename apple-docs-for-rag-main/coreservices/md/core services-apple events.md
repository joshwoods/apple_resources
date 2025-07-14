

- Core Services
-  Apple Events 

API Collection

# Apple Events

Communicate messages across process boundaries that can be performed and responded to with a reply event.

## Overview

When a script that targets an application is executed, commands are sent to the application in the form of *Apple events*, a kind of interprocess message. Cocoa scripting helps you create scriptable applications by doing much of the work of receiving these Apple events, extracting information from them, and invoking methods in your scriptable classes.

## Topics

### Structures

func AECallObjectAccessor(DescType, UnsafePointer&lt;AEDesc>!, DescType, DescType, UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Invokes the appropriate object accessor function for a specific desired type and container type.

func AECheckIsRecord(UnsafePointer&lt;AEDesc>!) -> Bool

Determines whether a descriptor is truly an `AERecord`.

func AECoerceDesc(UnsafePointer&lt;AEDesc>!, DescType, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Coerces the data in a descriptor to another descriptor type and creates a descriptor containing the newly coerced data.

func AECoercePtr(DescType, UnsafeRawPointer!, Size, DescType, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Coerces data to a desired descriptor type and creates a descriptor containing the newly coerced data.

func AECompareDesc(UnsafePointer&lt;AEDesc>!, UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;DarwinBoolean>!) -> OSStatus

func AECountItems(UnsafePointer&lt;AEDescList>!, UnsafeMutablePointer&lt;Int>!) -> OSErr

Counts the number of descriptors in a descriptor list.

func AECreateAppleEvent(AEEventClass, AEEventID, UnsafePointer&lt;AEAddressDesc>!, AEReturnID, AETransactionID, UnsafeMutablePointer&lt;AppleEvent>!) -> OSErr

Creates an Apple event with several important attributes but no parameters.

func AECreateDesc(DescType, UnsafeRawPointer!, Size, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a new descriptor that incorporates the specified data.

func AECreateDescFromExternalPtr(OSType, UnsafeRawPointer!, Size, AEDisposeExternalUPP!, SRefCon!, UnsafeMutablePointer&lt;AEDesc>!) -> OSStatus

Creates a new descriptor that uses a memory buffer supplied by the caller.

func AECreateList(UnsafeRawPointer!, Size, Bool, UnsafeMutablePointer&lt;AEDescList>!) -> OSErr

Creates an empty descriptor list or Apple event record.

func AECreateRemoteProcessResolver(CFAllocator!, CFURL!) -> AERemoteProcessResolverRef!

Creates an object for resolving a list of remote processes.

func AEDecodeMessage(UnsafeMutablePointer&lt;mach_msg_header_t>!, UnsafeMutablePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AppleEvent>!) -> OSStatus

Decodes a Mach message and converts it into an Apple event and its related reply.

func AEDeleteItem(UnsafeMutablePointer&lt;AEDescList>!, Int) -> OSErr

Deletes a descriptor from a descriptor list, causing all subsequent descriptors to move up one place.

func AEDeleteParam(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword) -> OSErr

Deletes a keyword-specified parameter from an Apple event record.

func AEDisposeDesc(UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Deallocates the memory used by a descriptor.

func AEDisposeRemoteProcessResolver(AERemoteProcessResolverRef!)

Disposes of an `AERemoteProcessResolverRef`.

func AEDisposeToken(UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Deallocates the memory used by a token.

func AEDuplicateDesc(UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a copy of a descriptor.

func AEFlattenDesc(UnsafePointer&lt;AEDesc>!, Ptr!, Size, UnsafeMutablePointer&lt;Size>!) -> OSStatus

Flattens the specified descriptor and stores the data in the supplied buffer.

func AEGetArray(UnsafePointer&lt;AEDescList>!, AEArrayType, AEArrayDataPointer!, Size, UnsafeMutablePointer&lt;DescType>!, UnsafeMutablePointer&lt;Size>!, UnsafeMutablePointer&lt;Int>!) -> OSErr

Extracts data from an Apple event array created with the `AEPutArray` function and stores it as a standard array of fixed size items in the specified buffer.

func AEGetAttributeDesc(UnsafePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Gets a copy of the descriptor for a specified Apple event attribute from an Apple event; typically used when your application needs to pass the descriptor on to another function.

func AEGetAttributePtr(UnsafePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeMutablePointer&lt;DescType>!, UnsafeMutableRawPointer!, Size, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets a copy of the data for a specified Apple event attribute from an Apple event; typically used when your application needs to work with the data directly.

func AEGetCoercionHandler(DescType, DescType, UnsafeMutablePointer&lt;AECoercionHandlerUPP?>!, UnsafeMutablePointer&lt;SRefCon?>!, UnsafeMutablePointer&lt;DarwinBoolean>!, Bool) -> OSErr

Gets the coercion handler for a specified descriptor type.

func AEGetDescData(UnsafePointer&lt;AEDesc>!, UnsafeMutableRawPointer!, Size) -> OSErr

Gets the data from the specified descriptor.

func AEGetDescDataRange(UnsafePointer&lt;AEDesc>!, UnsafeMutableRawPointer!, Size, Size) -> OSStatus

Retrieves a specified series of bytes from the specified descriptor.

func AEGetDescDataSize(UnsafePointer&lt;AEDesc>!) -> Size

Gets the size, in bytes, of the data in the specified descriptor.

func AEGetEventHandler(AEEventClass, AEEventID, UnsafeMutablePointer&lt;AEEventHandlerUPP?>!, UnsafeMutablePointer&lt;SRefCon?>!, Bool) -> OSErr

Gets an event handler from an Apple event dispatch table.

func AEGetNthDesc(UnsafePointer&lt;AEDescList>!, Int, DescType, UnsafeMutablePointer&lt;AEKeyword>!, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Copies a descriptor from a specified position in a descriptor list into a specified descriptor; typically used when your application needs to pass the extracted data to another function as a descriptor.

func AEGetNthPtr(UnsafePointer&lt;AEDescList>!, Int, DescType, UnsafeMutablePointer&lt;AEKeyword>!, UnsafeMutablePointer&lt;DescType>!, UnsafeMutableRawPointer!, Size, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets a copy of the data from a descriptor at a specified position in a descriptor list; typically used when your application needs to work with the extracted data directly.

func AEGetObjectAccessor(DescType, DescType, UnsafeMutablePointer&lt;OSLAccessorUPP?>!, UnsafeMutablePointer&lt;SRefCon?>!, Bool) -> OSErr

Gets an object accessor function from an object accessor dispatch table.

func AEGetParamDesc(UnsafePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Gets a copy of the descriptor for a keyword-specified Apple event parameter from an Apple event or an Apple event record.

func AEGetParamPtr(UnsafePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeMutablePointer&lt;DescType>!, UnsafeMutableRawPointer!, Size, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets a copy of the data for a specified Apple event parameter from an Apple event or an Apple event record.

func AEGetRegisteredMachPort() -> mach_port_t

Returns the Mach port (in the form of a `mach_port_t`) that was registered with the bootstrap server for this process.

func AEGetSpecialHandler(AEKeyword, UnsafeMutablePointer&lt;AEEventHandlerUPP?>!, Bool) -> OSErr

Gets a specified handler from a special handler dispatch table.

func AEInitializeDesc(UnsafeMutablePointer&lt;AEDesc>!)

Initializes a new descriptor.

func AEInstallCoercionHandler(DescType, DescType, AECoercionHandlerUPP!, SRefCon!, Bool, Bool) -> OSErr

Installs a coercion handler in either the application or system coercion handler dispatch table.

func AEInstallEventHandler(AEEventClass, AEEventID, AEEventHandlerUPP!, SRefCon!, Bool) -> OSErr

Adds an entry for an event handler to an Apple event dispatch table.

func AEInstallObjectAccessor(DescType, DescType, OSLAccessorUPP!, SRefCon!, Bool) -> OSErr

Adds or replaces an entry for an object accessor function to an object accessor dispatch table.

func AEInstallSpecialHandler(AEKeyword, AEEventHandlerUPP!, Bool) -> OSErr

Installs a callback function in a special handler dispatch table.

func AEManagerInfo(AEKeyword, UnsafeMutablePointer&lt;Int>!) -> OSErr

Provides information about the version of the Apple Event Manager currently available or the number of processes that are currently recording Apple events.

func AEObjectInit() -> OSErr

Initializes the Object Support Library.

func AEPrintDescToHandle(UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;Handle?>!) -> OSStatus

Provides a pretty printer facility for displaying the contents of Apple event descriptors.

func AEProcessMessage(UnsafeMutablePointer&lt;mach_msg_header_t>!) -> OSStatus

Decodes and dispatches a low level Mach message event to an event handler, including packaging and returning the reply to the sender.

func AEPutArray(UnsafeMutablePointer&lt;AEDescList>!, AEArrayType, UnsafePointer&lt;AEArrayData>!, DescType, Size, Int) -> OSErr

Inserts the data for an Apple event array into a descriptor list, replacing any previous descriptors in the list.

func AEPutAttributeDesc(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, UnsafePointer&lt;AEDesc>!) -> OSErr

Adds a descriptor and a keyword to an Apple event as an attribute.

func AEPutAttributePtr(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeRawPointer!, Size) -> OSErr

Adds a pointer to data, a descriptor type, and a keyword to an Apple event as an attribute.

func AEPutDesc(UnsafeMutablePointer&lt;AEDescList>!, Int, UnsafePointer&lt;AEDesc>!) -> OSErr

Adds a descriptor to any descriptor list, possibly replacing an existing descriptor in the list.

func AEPutParamDesc(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, UnsafePointer&lt;AEDesc>!) -> OSErr

Inserts a descriptor and a keyword into an Apple event or Apple event record as an Apple event parameter.

func AEPutParamPtr(UnsafeMutablePointer&lt;AppleEvent>!, AEKeyword, DescType, UnsafeRawPointer!, Size) -> OSErr

Inserts data, a descriptor type, and a keyword into an Apple event or Apple event record as an Apple event parameter.

func AEPutPtr(UnsafeMutablePointer&lt;AEDescList>!, Int, DescType, UnsafeRawPointer!, Size) -> OSErr

Inserts data specified in a buffer into a descriptor list as a descriptor, possibly replacing an existing descriptor in the list.

func AERemoteProcessResolverGetProcesses(AERemoteProcessResolverRef!, UnsafeMutablePointer&lt;CFStreamError>!) -> Unmanaged&lt;CFArray>!

Returns an array of objects containing information about processes running on a remote machine.

func AERemoteProcessResolverScheduleWithRunLoop(AERemoteProcessResolverRef!, CFRunLoop!, CFString!, AERemoteProcessResolverCallback!, UnsafePointer&lt;AERemoteProcessResolverContext>!)

Schedules a resolver for execution on a given run loop in a given mode.

func AERemoveCoercionHandler(DescType, DescType, AECoercionHandlerUPP!, Bool) -> OSErr

Removes a coercion handler from a coercion handler dispatch table.

func AERemoveEventHandler(AEEventClass, AEEventID, AEEventHandlerUPP!, Bool) -> OSErr

Removes an event handler entry from an Apple event dispatch table.

func AERemoveObjectAccessor(DescType, DescType, OSLAccessorUPP!, Bool) -> OSErr

Removes an object accessor function from an object accessor dispatch table.

func AERemoveSpecialHandler(AEKeyword, AEEventHandlerUPP!, Bool) -> OSErr

Removes a handler from a special handler dispatch table.

func AEReplaceDescData(DescType, UnsafeRawPointer!, Size, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Copies the specified data into the specified descriptor, replacing any previous data.

func AEResolve(UnsafePointer&lt;AEDesc>!, Int16, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Resolves an object specifier.

func AESendMessage(UnsafePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AppleEvent>!, AESendMode, Int) -> OSStatus

Sends an AppleEvent to a target process without some of the overhead required by `AESend`.

func AESetObjectCallbacks(OSLCompareUPP!, OSLCountUPP!, OSLDisposeTokenUPP!, OSLGetMarkTokenUPP!, OSLMarkUPP!, OSLAdjustMarksUPP!, OSLGetErrDescUPP!) -> OSErr

Specifies the object callback functions for your application.

func AESizeOfAttribute(UnsafePointer&lt;AppleEvent>!, AEKeyword, UnsafeMutablePointer&lt;DescType>!, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets the size and descriptor type of an Apple event attribute from a descriptor of type `AppleEvent`.

func AESizeOfFlattenedDesc(UnsafePointer&lt;AEDesc>!) -> Size

Returns the amount of buffer space needed to store the descriptor after flattening it.

func AESizeOfNthItem(UnsafePointer&lt;AEDescList>!, Int, UnsafeMutablePointer&lt;DescType>!, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets the data size and descriptor type of the descriptor at a specified position in a descriptor list.

func AESizeOfParam(UnsafePointer&lt;AppleEvent>!, AEKeyword, UnsafeMutablePointer&lt;DescType>!, UnsafeMutablePointer&lt;Size>!) -> OSErr

Gets the size and descriptor type of an Apple event parameter from a descriptor of type `AERecord` or `AppleEvent`.

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

func AEStreamWriteKeyDesc(AEStreamRef!, AEKeyword, DescType, UnsafeRawPointer!, Size) -> OSStatus

Writes a complete keyword/descriptor pair to an `AEStreamRef`.

func AEUnflattenDesc(UnsafeRawPointer!, UnsafeMutablePointer&lt;AEDesc>!) -> OSStatus

Unflattens the data in the passed buffer and creates a descriptor from it.

Deprecated

struct AEArrayData

Stores array information to be put into a descriptor listwith the `AEPutArray` functionor extracted from a descriptor list with the `AEGetArray` function.

struct AEBuildError

Defines a structure for storing additional error codeinformation for “AEBuild” routines.

struct AEDesc

Stores data and an accompanying descriptor type to formthe basic building block of all Apple Events.

struct AEKeyDesc

Associates a keyword with a descriptor to form a keyword-specifieddescriptor.

struct AERemoteProcessResolverContext

Supplied as a parameter when performing asynchronous resolutionof remote processes.

### Constants

let kAERemoteProcessNameKey: CFString!

Use this key to obtain the visible name of the remote process, in the localization supplied by the server, as a `CFStringRef`.

let kAERemoteProcessProcessIDKey: CFString!

Use this key to obtain the process ID of the remote process, if available; if so, returned as a `CFNumberRef`.

let kAERemoteProcessURLKey: CFString!

Use this key to obtain the full URL to the remote process, as a `CFURLRef`.

let kAERemoteProcessUserIDKey: CFString!

Use this key to obtain the user ID of the remote process, if available; if so, returned as a `CFNumberRef`.

### Data Types

typealias OSLAccessorProcPtr

Your object accessor function either finds elements or properties of an Apple event object.

typealias OSLAccessorUPP

Defines a data type for the universal procedure pointer for the `OSLAccessorProcPtr` callback function pointer.

typealias OSLAdjustMarksProcPtr

Defines a pointer to an adjust marks callback function. Your adjust marks function unmarks objects previously marked by a call to your marking function.

typealias OSLAdjustMarksUPP

Defines a data type for the universal procedure pointer for the `OSLAdjustMarksProcPtr` callback function pointer.

typealias OSLCompareProcPtr

Defines a pointer to an object comparison callback function. Your object comparison function compares one Apple event object to another or to the data for a descriptor.

typealias OSLCompareUPP

Defines a data type for the universal procedure pointer for the `OSLCompareProcPtr` callback function pointer.

typealias OSLCountProcPtr

Defines a pointer to an object counting callback function. Your object counting function counts the number of Apple event objects of a specified class in a specified container object.

typealias OSLCountUPP

Defines a data type for the universal procedure pointer for the `OSLCountProcPtr` callback function pointer.

typealias OSLDisposeTokenProcPtr

Defines a pointer to a dispose token callback function. Your dispose token function, required only if you use a complex token format, disposes of the specified token.

typealias OSLDisposeTokenUPP

Defines a data type for the universal procedure pointer for the `OSLDisposeTokenProcPtr` callback function pointer.

typealias OSLGetErrDescProcPtr

Defines a pointer to an error descriptor callback function. Your error descriptor callback function supplies a pointer to an address where the Apple Event Manager can store the current descriptor if an error occurs during a call to the `AEResolve` function.

typealias OSLGetErrDescUPP

Defines a data type for the universal procedure pointer for the `OSLGetErrDescProcPtr` callback function pointer.

typealias OSLGetMarkTokenProcPtr

Defines a pointer to a mark token callback function. Your mark token function returns a mark token.

typealias OSLGetMarkTokenUPP

Defines a data type for the universal procedure pointer for the `OSLGetMarkTokenProcPtr` callback function pointer.

typealias OSLMarkProcPtr

Defines a pointer to an object marking callback function. Your object-marking function marks a specific Apple event object.

typealias OSLMarkUPP

Defines a data type for the universal procedure pointer for the `OSLMarkProcPtr` callback function pointer.

typealias AEAddressDesc

A descriptor that contains the address of an application, used to describe the target application for an Apple event.

typealias AEArrayDataPointer

A pointer to a union of type `AEArrayData`.

typealias AEArrayType

Stores a value that specifies an array type.

typealias AEBuildErrorCode

Represents syntax errors found by an Apple Event build routine.

typealias AECoerceDescProcPtr

Defines a pointer to a function that coerces data stored in a descriptor. Your descriptor coercion callback function coerces the data from the passed descriptor to the specified type, returning the coerced data in a second descriptor.

typealias AECoerceDescUPP

Defines a data type for the universal procedure pointer for the `AECoerceDescProcPtr` callback function pointer.

typealias AECoercePtrProcPtr

Defines a pointer to a function that coerces data stored in a buffer. Your pointer coercion callback routine coerces the data from the passed buffer to the specified type, returning the coerced data in a descriptor.

typealias AECoercePtrUPP

Defines a data type for the universal procedure pointer for the `AECoercePtrProcPtr` callback function pointer.

typealias AECoercionHandlerUPP

Defines a data type for the universal procedure pointer for the `AECoercionHandlerUPP` callback function pointer.

typealias AEDataStorage

A pointer to an opaque data type that provides storage for an `AEDesc` descriptor.

typealias AEDataStorageType

An opaque data type used to store data in Apple event descriptors.

typealias AEDescList

A descriptor whose data consists of a list of one or more descriptors.

typealias AEDescPtr

typealias AEDisposeExternalProcPtr

Defines a pointer to a function the Apple Event Manager calls to dispose of a descriptor created by the `AECreateDescFromExternalPtr` function. Your callback function disposes of the buffer you originally passed to that function.

typealias AEDisposeExternalUPP

Defines a universal procedure pointer to a function the Apple Event Manager calls to dispose of a descriptor created by the `AECreateDescFromExternalPtr` function.

typealias AEEventClass

Specifies the event class of an Apple event.

typealias AEEventHandlerProcPtr

Defines a pointer to a function that handles one or more Apple events. Your Apple event handler function performs any action requested by the Apple event, adds parameters to the reply Apple event if appropriate (possibly including error information), and returns a result code.

typealias AEEventHandlerUPP

Defines a data type for the universal procedure pointer for the `AEEventHandlerUPP` callback function pointer.

typealias AEEventID

Specifies the event ID of an Apple event.

typealias AEEventSource

A data type for values that specify how an Apple event was delivered.

typealias AEKeyword

A four-character code that uniquely identifies a descriptor in an Apple event record or an Apple event.

typealias AERecord

A descriptor whose data is a list of keyword-specified descriptors.

typealias AERemoteProcessResolverCallback

Defines a pointer to a function the Apple Event Manager calls when the asynchronous execution of a remote process resolver completes, either due to success or failure, after a call to the `AERemoteProcessResolverScheduleWithRunLoop` function. Your callback function can use the reference passed to it to get the remote process information.

typealias AERemoteProcessResolverRef

An opaque reference to an object that encapsulates the mechanism for obtaining a list of processes running on a remote machine.

typealias AEReturnID

Specifies a return ID for a created Apple event.

typealias AESendMode

Specify send preferences to the `AESend` function.

typealias AESendPriority

Specifies the processing priority for a sent Apple event.

typealias AEStreamRef

An opaque data structure for storing stream-based descriptor data.

typealias AETransactionID

Specifies a transaction ID.

### Enumerations

kAEDebugPOSTHeader

kAEHandleArray

kAEISGetURL

kAEISHTTPSearchArgs

kAEInfo

kAEInternetSuite

kAELogOut

kAEMenuClass

kAEMouseClass

kAENonmodifiable

kAEQDNotOr

kAESetPosition

kAESocks4Protocol

kAEUTHasReturningParam

kAEUseHTTPProxyAttr

Web Services Proxy support—these constants should be added as attributes of the event that is being sent (not as part of the direct object).

kAEUseSocksAttr

kAEUserTerminology

kAEZoomIn

keyAEAngle

keyAEBaseAddr

keyAEDoScale

keyAEHiliteRange

keyAEKeyword

keyAESuiteID

keyMenuID

keyMiscellaneous

keyReplyPortAttr

keySOAPStructureMetaData

keyUserNameAttr

Apple Event Recording Event ID Constants

Specify event IDs for events that deal with Apple event recording.

Callback Constants for the AEResolve Function

Specify supported callback features to the `AEResolve` function.

Constants for Object Specifiers, Positions, and Logical and Comparison Operations

Specify the types of the four keyword-specified descriptors that make up the data in an object specifier, as well as constants for position, logical operations, and comparison operations.

Data Array Constants

Specify an array type for storing or extracting descriptor lists with the `AEPutArray` and `AEGetArray` functions.

Descriptor Type Constants

Specify types for descriptors.

Event Class Constants

Specify the event class for an Apple event.

Event ID Constants

Specify the event ID for an Apple event.

Event Source Constants

Identify how an Apple event was delivered.

Factoring Constants

ID Constants for the AECreateAppleEvent Function

Specify values for the ID parameters of the `AECreateAppleEvent` function.

Key Form and Descriptor Type Object Specifier Constants

Specify possible values for the `keyAEKeyForm` field of an object specifier, as well as descriptor types used in resolving object specifiers.

Keyword Attribute Constants

Specify keyword values for Apple event attributes.

Keyword Parameter Constants

Specify keyword values for Apple event parameters, as well as information for the `AEManagerInfo` function to retrieve. Some common key word values are shown here.

Launch Apple Event Constants

In a `kAEOpenApplication` event, specify information about how the receiving application was launched.

Numeric Descriptor Type Constants

Specify types for numeric descriptors.

Object Class ID Constants

Specify the object class for an Apple event object.

Other Descriptor Type Constants

Specify types for Boolean and character descriptors.

Priority Constants for the AESend Function (Deprecated in macOS)

Specify a value for the `sendPriority` parameter of the `AESend` function.

Special Handler Callback Constants

Specify an object callback function to install, get, or remove from the special handler dispatch table.

Timeout Constants

Specify a timeout value.

## See Also

### Related Documentation

Cocoa Scripting Guide

