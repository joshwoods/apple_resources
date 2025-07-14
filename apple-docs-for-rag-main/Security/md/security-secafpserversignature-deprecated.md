

- Security
-  SecAFPServerSignature Deprecated

Type Alias

# SecAFPServerSignature

Represents a 16-byte Apple File Protocol server signature block.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias SecAFPServerSignature = (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)
```

Deprecated

Use internet password items instead of AppleShare password items.

## Discussion

Important

This type is deprecated. Use internet password items instead of AppleShare password items.

This type represents a 16-byte Apple File Protocol server signature block. You can use a value of this type with the keychain item attribute constant SecItemAttr.signatureItemAttr to specify an Apple File Protocol server signature.

