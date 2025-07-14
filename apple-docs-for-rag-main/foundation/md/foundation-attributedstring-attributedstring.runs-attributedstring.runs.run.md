

- Foundation
- AttributedString
- AttributedString.Runs
-  AttributedString.Runs.Run 

Structure

# AttributedString.Runs.Run

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@dynamicMemberLookup
struct Run
```

## Topics

### Instance Properties

var attributes: AttributeContainer

var range: Range&lt;AttributedString.Index>

### Subscripts

subscript&lt;K>(K.Type) -> K.Value?

subscript&lt;S>(dynamicMember _: KeyPath&lt;AttributeScopes, S.Type>) -> ScopedAttributeContainer&lt;S>

subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> K.Value?

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Sendable

