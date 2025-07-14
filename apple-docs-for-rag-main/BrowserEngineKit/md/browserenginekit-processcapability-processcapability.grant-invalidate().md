

- BrowserEngineKit
- ProcessCapability
- ProcessCapability.Grant
-  invalidate() 

Instance Method

# invalidate()

Invalidates the grant, removing the capability from the process it was granted to.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
func invalidate()
```

## Mentioned in 

Managing the browser extension life cycle

## See Also

### Testing and changing validity

var isValid: Bool

A Boolean that indicates whether the operating system has granted the capability to the browser extension process.

