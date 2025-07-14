

- BrowserEngineKit
- ProcessCapability
-  ProcessCapability.Grant 

Structure

# ProcessCapability.Grant

An object that represents a granted capability.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
struct Grant
```

## Mentioned in 

Managing the browser extension life cycle

## Topics

### Testing and changing validity

var isValid: Bool

A Boolean that indicates whether the operating system has granted the capability to the browser extension process.

func invalidate()

Invalidates the grant, removing the capability from the process it was granted to.

## See Also

### Granting capabilities to browser extension processes

case background

The operating system permits the helper extension process to run in the background to finish work.

case foreground

The operating system permits the helper extension process to run at foreground priority to work on behalf of the browser app.

case suspended

The operating system permits the helper extension process to remain resident in a suspended state.

case mediaPlaybackAndCapture(environment: MediaEnvironment)

The helper extension process may access media hardware required for media capture and playback.

