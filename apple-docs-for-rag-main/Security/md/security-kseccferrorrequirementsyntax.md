

- Security
-  kSecCFErrorRequirementSyntax 

Global Variable

# kSecCFErrorRequirementSyntax

A key whose value is a string containing a compilation error generated when parsing a requirement.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCFErrorRequirementSyntax: CFString
```

## Discussion

This key is present when a call to the SecRequirementCreateWithStringAndErrors(_:_:_:_:) function results in a compilation error during the processing of the code requirement string.

