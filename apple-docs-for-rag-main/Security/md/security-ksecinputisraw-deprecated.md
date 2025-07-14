

- Security
-  kSecInputIsRaw Deprecated

Global Variable

# kSecInputIsRaw

The input is raw.

macOS 10.7–13.0Deprecated

``` source
let kSecInputIsRaw: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

Using this type of input can be cryptographically unsafe (for example if you don’t blind a DSA or ECDSA signature you give away the key very quickly). You are strongly discouraged from using it..

