

- BrowserEngineKit
- ProcessCapability
-  ProcessCapability.suspended 

Case

# ProcessCapability.suspended

The operating system permits the helper extension process to remain resident in a suspended state.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
case suspended
```

## Overview

While a helper extension process has this capability, the operating system doesn’t grant it CPU time.

## See Also

### Granting capabilities to browser extension processes

case background

The operating system permits the helper extension process to run in the background to finish work.

case foreground

The operating system permits the helper extension process to run at foreground priority to work on behalf of the browser app.

case mediaPlaybackAndCapture(environment: MediaEnvironment)

The helper extension process may access media hardware required for media capture and playback.

struct Grant

An object that represents a granted capability.

