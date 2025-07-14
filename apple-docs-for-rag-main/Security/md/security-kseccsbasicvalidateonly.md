

- Security
-  kSecCSBasicValidateOnly 

Global Variable

# kSecCSBasicValidateOnly

Do not validate either the main executable or the bundle resources, if any.

Mac Catalyst 13.0+macOS 10.0+

``` source
var kSecCSBasicValidateOnly: UInt32 { get }
```

## Discussion

This flag is the bitwise OR of the kSecCSDoNotValidateExecutable and kSecCSDoNotValidateResources flags.

