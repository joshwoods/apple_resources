

- BrowserEngineKit
- ProcessCapability
-  ProcessCapability.background 

Case

# ProcessCapability.background

The operating system permits the helper extension process to run in the background to finish work.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
case background
```

## See Also

### Granting capabilities to browser extension processes

case foreground

The operating system permits the helper extension process to run at foreground priority to work on behalf of the browser app.

case suspended

The operating system permits the helper extension process to remain resident in a suspended state.

case mediaPlaybackAndCapture(environment: MediaEnvironment)

The helper extension process may access media hardware required for media capture and playback.

struct Grant

An object that represents a granted capability.

