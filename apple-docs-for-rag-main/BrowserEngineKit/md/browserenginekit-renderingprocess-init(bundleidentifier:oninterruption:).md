

- BrowserEngineKit
- RenderingProcess
-  init(bundleIdentifier:onInterruption:) 

Initializer

# init(bundleIdentifier:onInterruption:)

Launches a rendering extension process asynchronously.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
init(
    bundleIdentifier: String? = nil,
    onInterruption: @escaping () -> Void
) async throws
```

## Parameters 

`bundleIdentifier`  

The bundle identifier of the rendering extension to launch, or `nil` to use the default bundle identifier for this app’s rendering extension.

`onInterruption`  

A block that the operating system calls if the rendering extension process exits abnormally.

## Overview

Your web browser app can run one instance of each of its rendering extensions. The first time you initialize this object, the operating system launches your rendering extension. If you subsequently initialize new instances of `RenderingProcess` using the same bundle identifier, they refer to the same process.

The operating system guarantees that the process launched when this initializer returns.

## See Also

### Creating and invalidating extension processes

func invalidate()

Stops the extension process.

