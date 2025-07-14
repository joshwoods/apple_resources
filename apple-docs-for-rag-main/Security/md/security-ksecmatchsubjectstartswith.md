

- Security
-  kSecMatchSubjectStartsWith 

Global Variable

# kSecMatchSubjectStartsWith

A key whose value is a string to match against the beginning of a certificate or identity’s subject.

macOS 10.7+

``` source
let kSecMatchSubjectStartsWith: CFString
```

## Discussion

The corresponding value is of type CFString. If provided, returned certificates or identities are limited to those whose subject starts with this string.

