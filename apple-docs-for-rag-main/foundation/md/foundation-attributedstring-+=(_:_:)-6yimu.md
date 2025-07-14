

- Foundation
- AttributedString
-  +=(\_:\_:) 

Operator

# +=(\_:\_:)

Appends an attributed string or substring to another attributed string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func += (lhs: inout AttributedString, rhs: some AttributedStringProtocol)
```

## Parameters 

`lhs`  

An attributed string. After the operation, the value of this string is the original `lhs` string with `rhs` appended to it.

`rhs`  

An attributed string or substring to append to `lhs`.

## See Also

### Combining Attributed Strings

func append(some AttributedStringProtocol)

Appends a string to the attributed string.

static func + (AttributedString, AttributedString) -> AttributedString

Concatenates two attributed strings.

static func + (AttributedString, some AttributedStringProtocol) -> AttributedString

Concatenates two attributed strings or substrings.

static func += (inout AttributedString, AttributedString)

Appends an attributed string to another attributed string.

