

- Security
- SecCodeSignatureFlags
-  adhoc 

Type Property

# adhoc

Must be used without a signing identity.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var adhoc: SecCodeSignatureFlags { get }
```

## Discussion

The code has been sealed without a signing identity. No identity may be retrieved from it, and any code requirement placing restrictions on the signing identity will fail. This flag is set by Code Signing Services when you create an ad-hoc signature, and cannot be set explicitly. An ad-hoc signature is created by signing with the pseudo-identity “-” (a dash).

