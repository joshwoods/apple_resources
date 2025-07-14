

- Core Services
- Launch Services
-  LSLaunchFlags 

Structure

# LSLaunchFlags

The specification for launching an app.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct LSLaunchFlags
```

## Overview

They are passed in a launch specification structure (`LSLaunchFSRefSpec` to the `LSOpenFromRefSpec` function or `LSLaunchURLSpec` to the `LSOpenFromURLSpec` function), to control the manner in which apps are launched.

## Topics

### Creating Application Launch Flags

init(rawValue: OptionBits)

### Constants

static var defaults: LSLaunchFlags

Requests launching in the default manner (as if the only flags set were `kLSLaunchNoParams`, `kLSLaunchAsync`, and `kLSLaunchStartClassic`).

static var andPrint: LSLaunchFlags

Requests that documents opened in the application be printed.

static var andDisplayErrors: LSLaunchFlags

Requests that launch and open failures be displayed in the UI.

static var dontAddToRecents: LSLaunchFlags

Requests that the application or documents not be added to the Finder’s Recent Items menu.

static var dontSwitch: LSLaunchFlags

Requests that the application be launched without being brought to the foreground.

static var async: LSLaunchFlags

Requests that the application be launched asynchronously.

static var newInstance: LSLaunchFlags

Requests that a new instance of the application be started, even if one is already running.

static var andHide: LSLaunchFlags

Requests that the application be hidden as soon as it completes its launch sequence.

static var andHideOthers: LSLaunchFlags

Requests that other applications be hidden as soon as the opened application completes its launch sequence.

## Relationships

### Conforms To

- OptionSet
- Sendable

