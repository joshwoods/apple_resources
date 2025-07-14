

- Security
-  kSecMatchSubjectWholeString 

Global Variable

# kSecMatchSubjectWholeString

A key whose value is a string to exactly match a certificate or identity’s subject.

macOS 10.7+

``` source
let kSecMatchSubjectWholeString: CFString
```

## Discussion

The corresponding value is of type CFString. If provided, returned certificates or identities are limited to those whose subject is exactly equal to this string.

