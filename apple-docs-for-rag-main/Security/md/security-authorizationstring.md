

- Security
-  AuthorizationString 

Type Alias

# AuthorizationString

A zero-terminated string in UTF-8 encoding.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AuthorizationString = UnsafePointer
```

## Discussion

Use this in a call to the AuthorizationCopyInfo(_:_:_:) function for the `tag` parameter.

