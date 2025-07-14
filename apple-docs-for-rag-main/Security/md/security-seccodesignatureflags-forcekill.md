

- Security
- SecCodeSignatureFlags
-  forceKill 

Type Property

# forceKill

Always set the termination status flag on launch.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var forceKill: SecCodeSignatureFlags { get }
```

## Discussion

The `kSecCodeStatusKill` flag indicates that the code wishes to be terminated if it is ever invalidated. Once this is set, it cannot be cleared. Therefore, setting this option flag guarantees that the running code will always be valid, since it will die immediately if it becomes invalid.

