

- BrowserEngineKit
- ProcessCapability
- ProcessCapability.Grant
-  isValid 

Instance Property

# isValid

A Boolean that indicates whether the operating system has granted the capability to the browser extension process.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
var isValid: Bool { get }
```

## Overview

If the operating system has granted this capability to the browser extension process and you haven’t called invalidate(), then this property’s value is `true`; otherwise, it’s false.

## See Also

### Testing and changing validity

func invalidate()

Invalidates the grant, removing the capability from the process it was granted to.

