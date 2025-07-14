

- Core Services
- Launch Services
-  LSRequestedInfo 

Structure

# LSRequestedInfo

The specification that controls which information to obtain about an item.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct LSRequestedInfo
```

## Overview

These flags are passed to the `LSCopyItemInfoForRef` and `LSCopyItemInfoForURL` functions to specify the type of information to be obtained in an item-information record; see LSItemInfoRecord for a description of this structure.

## Topics

### Creating an Item Information Request

init(rawValue: OptionBits)

### Constants

static var requestExtension: LSRequestedInfo

Requests the item’s filename extension.

Deprecated

static var requestTypeCreator: LSRequestedInfo

Requests the item’s file type and creator signature.

Deprecated

static var requestBasicFlagsOnly: LSRequestedInfo

Requests all item-information flags that are not application-specific: that is, all except `kLSItemInfoIsNativeApp` through `kLSItemInfoAppIsScriptable`.

Deprecated

static var requestAppTypeFlags: LSRequestedInfo

Requests all application-specific item-information flags: that is, `kLSItemInfoIsNativeApp` through `kLSItemInfoAppIsScriptable`.

Deprecated

static var requestAllFlags: LSRequestedInfo

Requests all item-information flags.

Deprecated

static var requestIconAndKind: LSRequestedInfo

Not used.

Deprecated

static var requestExtensionFlagsOnly: LSRequestedInfo

Requests only the `kLSItemInfoExtensionIsHidden` item-information flag.

Deprecated

static var requestAllInfo: LSRequestedInfo

Requests all available item information.

Deprecated

## Relationships

### Conforms To

- OptionSet
- Sendable

