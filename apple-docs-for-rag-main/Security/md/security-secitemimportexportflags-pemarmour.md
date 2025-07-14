

- Security
- SecItemImportExportFlags
-  pemArmour 

Type Property

# pemArmour

A flag that indicates the exported data should have PEM armor.

macOS 10.0+

``` source
static var pemArmour: SecItemImportExportFlags { get }
```

## Discussion

PEM armor refers to a way of expressing binary data as an ASCII string so that it can be transferred over text-only channels such as email. (PEM stands for an Internet standard, Privacy Enhanced Mail.)

