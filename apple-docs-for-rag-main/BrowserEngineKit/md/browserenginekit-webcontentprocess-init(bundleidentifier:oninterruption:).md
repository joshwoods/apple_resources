

- BrowserEngineKit
- WebContentProcess
-  init(bundleIdentifier:onInterruption:) 

Initializer

# init(bundleIdentifier:onInterruption:)

Launches a web content process asynchronously.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
init(
    bundleIdentifier: String? = nil,
    onInterruption: @escaping () -> Void
) async throws
```

## Parameters 

`bundleIdentifier`  

The bundle identifier of the content extension to launch, or `nil` to use the default bundle identifier for this app’s web content extension.

`onInterruption`  

A block that the operating system calls if the web content extension process exits abnormally.

## Overview

Initializing a `WebContentProcess` object launches a new instance of the web content extension. The operating system guarantees that the process launched when this initializer returns.

## See Also

### Creating and invalidating extension processes

func invalidate()

Stops the extension process.

