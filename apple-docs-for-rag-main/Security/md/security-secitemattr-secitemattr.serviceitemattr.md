

- Security
- SecItemAttr
-  SecItemAttr.serviceItemAttr 

Case

# SecItemAttr.serviceItemAttr

Identifies the service attribute.

Mac Catalyst 13.0+macOS 10.0+

``` source
case serviceItemAttr
```

## Discussion

You use this tag to set or get a string that represents the service associated with this item, for example, “iTools”. This is unique to generic password attributes. Keychain strings should use UTF-8 encoding.

