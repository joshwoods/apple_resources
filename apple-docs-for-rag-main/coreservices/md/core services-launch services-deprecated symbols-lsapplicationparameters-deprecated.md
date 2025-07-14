

- Core Services
- Launch Services
- Deprecated Symbols
-  LSApplicationParameters Deprecated

Structure

# LSApplicationParameters

The specification that defines the app, launch flags, and additional parameters that control how an app launches.

macOS 10.4–10.10Deprecated

``` source
struct LSApplicationParameters
```

## Overview

This structure is passed as a parameter to LSOpenApplication(_:_:), LSOpenItemsWithRole(_:_:_:_:_:_:_:), and LSOpenURLsWithRole(_:_:_:_:_:_:).

## Topics

### Initializers

init()

init(version: CFIndex, flags: LSLaunchFlags, application: UnsafePointer&lt;FSRef>!, asyncLaunchRefCon: UnsafeMutableRawPointer!, environment: Unmanaged&lt;CFDictionary>!, argv: Unmanaged&lt;CFArray>!, initialEvent: UnsafeMutablePointer&lt;AppleEvent>!)

### Instance Properties

var application: UnsafePointer&lt;FSRef>!

The `FSRef` ofthe application to open.

var argv: Unmanaged&lt;CFArray>!

An array of values of type `CFString` that specify the arguments that are to be passed to `main()` in the launched process. The value of this field can be `NULL`. This field is ignored in macOS 10.4.

var asyncLaunchRefCon: UnsafeMutableRawPointer!

The client `refCon` thatis to appear in subsequent launch notifications.

var environment: Unmanaged&lt;CFDictionary>!

A dictionary of `CFStringRef` keysand values for environment variables to set in the launched process.The value of this field can be `NULL`.

var flags: LSLaunchFlags

Launch flags. For possible values, see LSLaunchFlags.

var initialEvent: UnsafeMutablePointer&lt;AppleEvent>!

The first Apple Event to send to the launchedprocess. The value of this field can be `NULL`.

var version: CFIndex

The version of the structure. The value of thisfield must be `0`.

## See Also

### Deprecated Structures

struct LSLaunchFSRefSpec

The specification that defines, by file-system reference, an app to launch, items to open, or both, along with related information.

Deprecated

struct LSItemInfoRecord

The specification that contains requested information about an item.

Deprecated

