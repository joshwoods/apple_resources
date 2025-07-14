

- Security
-  kSecIVKey Deprecated

Global Variable

# kSecIVKey

The setting for an initialization vector.

macOS 10.7–13.0Deprecated

``` source
let kSecIVKey: CFString
```

Deprecated

SecTransform is no longer supported

## Discussion

The key’s associated value is an initialization vector. Provide random bytes for this value—for example, created by calling the SecRandomCopyBytes(_:_:_:) method—unless your specification requires something else. The number of bytes in the vector should match the block size of the underlying block cipher. For example, use 16 bytes for AES encryption.

If you don’t supply a value for this key, any operations that require an initialization vector use a value of zero by default, which can compromise the security of your encryption.

