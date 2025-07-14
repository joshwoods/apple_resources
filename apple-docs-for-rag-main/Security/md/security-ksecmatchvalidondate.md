

- Security
-  kSecMatchValidOnDate 

Global Variable

# kSecMatchValidOnDate

A key whose value indicates the validity date.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecMatchValidOnDate: CFString
```

## Discussion

The corresponding value is of type CFDate. If provided, returned keys, certificates or identities are limited to those that are valid for the given date. Pass a value of kCFNull to indicate the current date.

