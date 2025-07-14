

- Core Services
- Launch Services
- Deprecated Symbols
-  LSItemInfoRecord Deprecated

Structure

# LSItemInfoRecord

The specification that contains requested information about an item.

Mac Catalyst 13.0–13.1DeprecatedmacOS 10.0–10.11Deprecated

``` source
struct LSItemInfoRecord
```

## Overview

This data type defines an item-information record used bythe `LSCopyItemInfoForRef` and `LSCopyItemInfoForURL` functionsto return requested information about an item.

## Topics

### Initializers

init()

init(flags: LSItemInfoFlags, filetype: OSType, creator: OSType, extension: Unmanaged&lt;CFString>!)

### Instance Properties

var creator: OSType

The item’s creator signature.

var `extension`: Unmanaged&lt;CFString>!

A Core Foundation string object specifying theitem’s filename extension; see the *CFString Reference* inthe Core Foundation Reference Documentation for a description ofthe `CFStringRef` datatype.

var filetype: OSType

The item’s file type.

var flags: LSItemInfoFlags

Item-information flags specifying informationabout the item; see LSItemInfoFlags for a description of these flags.

## See Also

### Deprecated Structures

struct LSApplicationParameters

The specification that defines the app, launch flags, and additional parameters that control how an app launches.

Deprecated

struct LSLaunchFSRefSpec

The specification that defines, by file-system reference, an app to launch, items to open, or both, along with related information.

Deprecated

