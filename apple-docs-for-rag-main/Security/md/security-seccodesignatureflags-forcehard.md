

- Security
- SecCodeSignatureFlags
-  forceHard 

Type Property

# forceHard

Always set the hard status flag on launch.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var forceHard: SecCodeSignatureFlags { get }
```

## Discussion

The `kSecCodeStatusHard` flag indicates that the code prefers to be denied access to a resource if gaining such access would cause its invalidation. Once the hard bit is set, it cannot be cleared. Therefore, setting this option flag guarantees that the code will always have the `kSecCodeStatusHard` flag set.

