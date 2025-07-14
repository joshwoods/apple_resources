

- Core Foundation
-  CFPlugIn 

Class

# CFPlugIn

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFPlugIn
```

## Overview

`CFPlugIn` provides a standard architecture for application extensions. With `CFPlugIn`, you can design your application as a host framework that uses a set of executable code modules called plug-ins to provide certain well-defined areas of functionality. This approach allows third-party developers to add features to your application without requiring access to your source code. You can also bundle together plug-ins for multiple platforms and let `CFPlugIn` transparently load the appropriate plug-in at runtime. You can use `CFPlugIn` to add plug-in capability to, or write a plug-in for, your application.

## Topics

### Creating Plug-ins

func CFPlugInCreate(CFAllocator!, CFURL!) -> CFPlugIn!

Creates a CFPlugIn given its URL.

func CFPlugInInstanceCreate(CFAllocator!, CFUUID!, CFUUID!) -> UnsafeMutableRawPointer!

Creates a `CFPlugIn` instance of a given type using a given factory.

### Registration

func CFPlugInRegisterFactoryFunction(CFUUID!, CFPlugInFactoryFunction!) -> Bool

Registers a factory function and its UUID with a `CFPlugIn` object.

func CFPlugInRegisterFactoryFunctionByName(CFUUID!, CFPlugIn!, CFString!) -> Bool

Registers a factory function with a `CFPlugIn` object using the function’s name instead of its UUID.

func CFPlugInRegisterPlugInType(CFUUID!, CFUUID!) -> Bool

Registers a type and its corresponding factory function with a `CFPlugIn` object.

func CFPlugInUnregisterFactory(CFUUID!) -> Bool

Removes the given function from a plug-in’s list of registered factory functions.

func CFPlugInUnregisterPlugInType(CFUUID!, CFUUID!) -> Bool

Removes the given type from a plug-in’s list of registered types.

### CFPlugIn Miscellaneous Functions

func CFPlugInAddInstanceForFactory(CFUUID!)

Registers a new instance of a type with `CFPlugIn`.

func CFPlugInFindFactoriesForPlugInType(CFUUID!) -> CFArray!

Searches all registered plug-ins for factory functions capable of creating an instance of the given type.

func CFPlugInFindFactoriesForPlugInTypeInPlugIn(CFUUID!, CFPlugIn!) -> CFArray!

Searches the given plug-in for factory functions capable of creating an instance of the given type.

func CFPlugInGetBundle(CFPlugIn!) -> CFBundle!

Returns a plug-in’s bundle.

func CFPlugInGetTypeID() -> CFTypeID

Returns the type identifier for the `CFPlugIn` opaque type.

func CFPlugInIsLoadOnDemand(CFPlugIn!) -> Bool

Determines whether or not a plug-in is loaded on demand.

func CFPlugInRemoveInstanceForFactory(CFUUID!)

Unregisters an instance of a type with `CFPlugIn`.

func CFPlugInSetLoadOnDemand(CFPlugIn!, Bool)

Enables or disables load on demand for plug-ins that do dynamic registration (only when a client requests an instance of a supported type).

### Callbacks

typealias CFPlugInDynamicRegisterFunction

A callback which provides a plug-in the opportunity to dynamically register its types with a host.

typealias CFPlugInFactoryFunction

Callback function that a plug-in author must implement to create a plug-in instance.

typealias CFPlugInUnloadFunction

Callback function that is called, if present, just before a plug-in’s code is unloaded.

### Constants

Information Property List Keys

A plug-in’s information property list can contain these keys used for registering types, factories, and interfaces.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

