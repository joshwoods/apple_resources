

- BrowserEngineKit
- ProcessCapability
-  ProcessCapability.mediaPlaybackAndCapture(environment:) 

Case

# ProcessCapability.mediaPlaybackAndCapture(environment:)

The helper extension process may access media hardware required for media capture and playback.

iOS 17.4+iPadOS 17.4+

``` source
case mediaPlaybackAndCapture(environment: MediaEnvironment)
```

## Discussion

Important

You need to call activate() on the media environment before you grant this capability to an extension.

## See Also

### Granting capabilities to browser extension processes

case background

The operating system permits the helper extension process to run in the background to finish work.

case foreground

The operating system permits the helper extension process to run at foreground priority to work on behalf of the browser app.

case suspended

The operating system permits the helper extension process to remain resident in a suspended state.

struct Grant

An object that represents a granted capability.

