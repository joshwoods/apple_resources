

- Security
-  kSecCSStrictValidate 

Global Variable

# kSecCSStrictValidate

Perform additional checks to ensure the validity of code in bundle form.

Mac Catalyst 13.0+macOS 10.0+

``` source
var kSecCSStrictValidate: UInt32 { get }
```

## Discussion

For code in bundle form, perform additional checks to verify that the bundle is not structured in a way that would allow tampering, and reject any resource envelope that introduces weaknesses into the signature.

