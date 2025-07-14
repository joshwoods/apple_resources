

- Swift
- StringProtocol
-  canBeConverted(to:) 

Instance Method

# canBeConverted(to:)

Returns a Boolean value that indicates whether the string can be converted to the specified encoding without loss of information.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func canBeConverted(to encoding: String.Encoding) -> Bool
```

## Parameters 

`encoding`  

A string encoding.

## Return Value

`true` if the string can be encoded in `encoding` without loss of information; otherwise, `false`.

