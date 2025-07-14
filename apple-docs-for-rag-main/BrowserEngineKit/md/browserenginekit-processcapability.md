

- BrowserEngineKit
-  ProcessCapability 

Enumeration

# ProcessCapability

An enumeration that identifies capabilities that a browser app can grant to its extension processes.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
enum ProcessCapability
```

## Mentioned in 

Managing the browser extension life cycle

## Overview

To grant a capability to an extension, call the `grantCapability(_:)` method for the relevant process:

Web content extension  
grantCapability(_:)

Networking extension  
grantCapability(_:)

Rendering extension  
grantCapability(_:)

These methods return a ProcessCapability.Grant object. When your extension no longer needs the capability, call invalidate().

## Topics

### Granting capabilities to browser extension processes

case background

The operating system permits the helper extension process to run in the background to finish work.

case foreground

The operating system permits the helper extension process to run at foreground priority to work on behalf of the browser app.

case suspended

The operating system permits the helper extension process to remain resident in a suspended state.

case mediaPlaybackAndCapture(environment: MediaEnvironment)

The helper extension process may access media hardware required for media capture and playback.

struct Grant

An object that represents a granted capability.

## See Also

### Extension capabilities

struct MediaEnvironment

An object that identifies a media playback or streaming environment.

