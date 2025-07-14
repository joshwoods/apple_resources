

- Security
- SecKeyImportExportFlags
-  noAccessControl 

Type Property

# noAccessControl

A flag that indicates imported private keys have no access object attached to them.

macOS 10.0+

``` source
static var noAccessControl: SecKeyImportExportFlags { get }
```

## Discussion

In the absence of both this bit and the accessRef field in the SecItemImportExportKeyParameters structure, imported private keys receive default access controls.

