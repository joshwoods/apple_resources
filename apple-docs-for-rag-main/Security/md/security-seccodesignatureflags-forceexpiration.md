

- Security
- SecCodeSignatureFlags
-  forceExpiration 

Type Property

# forceExpiration

Always set the considerExpiration flag when validating the code.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var forceExpiration: SecCodeSignatureFlags { get }
```

## Discussion

When passed to a function that performs code validation, the `kSecCSConsiderExpiration` flag requests that code signatures made by expired certificates be rejected. By default, expiration of participating certificates is not automatic grounds for rejection.

