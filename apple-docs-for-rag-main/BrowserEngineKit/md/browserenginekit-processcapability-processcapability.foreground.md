

- BrowserEngineKit
- ProcessCapability
-  ProcessCapability.foreground 

Case

# ProcessCapability.foreground

The operating system permits the helper extension process to run at foreground priority to work on behalf of the browser app.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
case foreground
```

## Mentioned in 

Managing the browser extension life cycle

## Overview

Use this capability while your browser app is in the foreground, to allow extensions that support the browser’s UI to run at foreground priority.

## See Also

### Granting capabilities to browser extension processes

case background

The operating system permits the helper extension process to run in the background to finish work.

case suspended

The operating system permits the helper extension process to remain resident in a suspended state.

case mediaPlaybackAndCapture(environment: MediaEnvironment)

The helper extension process may access media hardware required for media capture and playback.

struct Grant

An object that represents a granted capability.

