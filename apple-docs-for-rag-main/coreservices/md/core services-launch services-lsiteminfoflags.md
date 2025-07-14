

- Core Services
- Launch Services
-  LSItemInfoFlags 

Structure

# LSItemInfoFlags

The specification that provides information about an item.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct LSItemInfoFlags
```

## Overview

These flags are set in an item-information record to provide information about an item; see LSItemInfoRecord for a description of this structure.

## Topics

### Creating Item Information Flags

init(rawValue: OptionBits)

### Constants

static var isPlainFile: LSItemInfoFlags

Item is a data file (and not, for example, a directory, volume, or UNIX symbolic link).

Deprecated

static var isPackage: LSItemInfoFlags

Item is a packaged directory.

Deprecated

static var isApplication: LSItemInfoFlags

Item is a single-file or packaged application.

Deprecated

static var isContainer: LSItemInfoFlags

Item is a directory (includes packages) or volume.

Deprecated

static var isAliasFile: LSItemInfoFlags

Item is an alias file (includes symbolic links).

Deprecated

static var isSymlink: LSItemInfoFlags

Item is a UNIX symbolic link.

Deprecated

static var isInvisible: LSItemInfoFlags

Item is invisible, because either its name begins with a period or its `isInvisible` Finder flag is set.

Deprecated

static var isNativeApp: LSItemInfoFlags

Item is an application that can run natively in macOS.

Deprecated

static var isClassicApp: LSItemInfoFlags

Item is an application that cannot run natively and must be launched in the Classic emulation environment.

Deprecated

static var appPrefersNative: LSItemInfoFlags

Item is an application that can run either natively or in the Classic emulation environment, but prefers to be launched natively. This flag is valid only when `kLSItemInfoIsNativeApp` is set.

Deprecated

static var appPrefersClassic: LSItemInfoFlags

Item is an application that can run either natively or in the Classic emulation environment, but prefers tobe launched in the Classic environment. This flag is valid only when `kLSItemInfoIsNativeApp` isset.

Deprecated

static var appIsScriptable: LSItemInfoFlags

Item is an application that can be scripted.

Deprecated

static var isVolume: LSItemInfoFlags

Item is the root directory of a volume or mount point.

Deprecated

static var extensionIsHidden: LSItemInfoFlags

Item has a hidden filename extension.

Deprecated

## Relationships

### Conforms To

- OptionSet
- Sendable

