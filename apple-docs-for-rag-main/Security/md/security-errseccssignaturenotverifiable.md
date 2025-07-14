

- Security
-  errSecCSSignatureNotVerifiable 

Global Variable

# errSecCSSignatureNotVerifiable

Signature cannot be read.

Mac Catalyst 13.0+macOS 10.0+

``` source
var errSecCSSignatureNotVerifiable: OSStatus { get }
```

## Discussion

This error might be due to a filesystem that maps root to an unprivileged user, for example.

