

- Security
- SecItemAttr
-  SecItemAttr.addressItemAttr 

Case

# SecItemAttr.addressItemAttr

Identifies the address attribute.

Mac Catalyst 13.0+macOS 10.0+

``` source
case addressItemAttr
```

## Discussion

You use this tag to set or get a value of type `string` that represents the AppleTalk zone name, or the IP or domain name that represents the server address. This is unique to AppleShare password attributes. Keychain strings should use UTF-8 encoding.

