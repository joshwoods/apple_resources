

- Security
-  kSecMatchSubjectEndsWith 

Global Variable

# kSecMatchSubjectEndsWith

A key whose value is a string to match against the end of a certificate or identity’s subject.

macOS 10.7+

``` source
let kSecMatchSubjectEndsWith: CFString
```

## Discussion

The corresponding value is of type CFString. If provided, returned certificates or identities are limited to those whose subject ends with this string.

