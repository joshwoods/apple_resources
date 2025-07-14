

- Foundation
- AttributedString
-  append(\_:) 

Instance Method

# append(\_:)

Appends a string to the attributed string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func append(_ s: some AttributedStringProtocol)
```

## Parameters 

`s`  

The string to append.

## See Also

### Combining Attributed Strings

static func + (AttributedString, AttributedString) -> AttributedString

Concatenates two attributed strings.

static func + (AttributedString, some AttributedStringProtocol) -> AttributedString

Concatenates two attributed strings or substrings.

static func += (inout AttributedString, AttributedString)

Appends an attributed string to another attributed string.

static func += (inout AttributedString, some AttributedStringProtocol)

Appends an attributed string or substring to another attributed string.

