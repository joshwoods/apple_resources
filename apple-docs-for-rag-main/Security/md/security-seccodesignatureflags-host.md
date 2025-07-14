

- Security
- SecCodeSignatureFlags
-  host 

Type Property

# host

May host guest code.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var host: SecCodeSignatureFlags { get }
```

## Discussion

Indicates that the code may act as a host that controls and supervises guest code. If this flag is not set in a code signature, the code is never considered eligible to be a host, and any attempt to act like one is ignored or rejected.

