

- Foundation
- AttributedString
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Concatenates two attributed strings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func + (lhs: AttributedString, rhs: AttributedString) -> AttributedString
```

## Parameters 

`lhs`  

An attributed string to concatenate.

`rhs`  

Another attributed string to concatenate.

## Return Value

The result of concatenating `rhs` to the end of `lhs`.

## See Also

### Combining Attributed Strings

func append(some AttributedStringProtocol)

Appends a string to the attributed string.

static func + (AttributedString, some AttributedStringProtocol) -> AttributedString

Concatenates two attributed strings or substrings.

static func += (inout AttributedString, AttributedString)

Appends an attributed string to another attributed string.

static func += (inout AttributedString, some AttributedStringProtocol)

Appends an attributed string or substring to another attributed string.

