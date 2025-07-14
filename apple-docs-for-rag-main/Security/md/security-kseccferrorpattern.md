

- Security
-  kSecCFErrorPattern 

Global Variable

# kSecCFErrorPattern

A key whose value is a string containing a regular expression that’s part of a resource specification that did not parse correctly.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCFErrorPattern: CFString
```

## Discussion

A resource specification is an information property list (`Info.plist` file) that says which files are resources and which are not. This error is returned if any part of the resource specification can’t be parsed.

