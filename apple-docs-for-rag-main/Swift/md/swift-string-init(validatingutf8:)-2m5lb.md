

- Swift
- String
-  init(validatingUTF8:) 

Initializer

# init(validatingUTF8:)

Creates a new string by copying and validating the null-terminated UTF-8 data referenced by the given array.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+SwiftDeprecated

``` source
init?(validatingUTF8 cString: [CChar])
```

## Parameters 

`cString`  

An array containing a null-terminated sequence of UTF-8 code units.

## Discussion

This initializer does not try to repair ill-formed UTF-8 code unit sequences. If any are found, the result of the initializer is `nil`.

Note

This initializer is deprecated. Use the initializer `String.init?(validating: array, as: UTF8.self)` instead, remembering that “\0” is a valid character in Swift.

