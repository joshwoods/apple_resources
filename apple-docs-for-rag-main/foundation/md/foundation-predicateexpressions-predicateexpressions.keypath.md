

- Foundation
- PredicateExpressions
-  PredicateExpressions.KeyPath 

Structure

# PredicateExpressions.KeyPath

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct KeyPath where Root : PredicateExpression
```

## Topics

### Initializers

init(root: Root, keyPath: any KeyPath&lt;Root.Output, Output> &amp; Sendable)

### Instance Properties

let keyPath: any KeyPath&lt;Root.Output, Output> &amp; Sendable

var kind: PredicateExpressions.KeyPath&lt;Root, Output>.CommonKeyPathKind?

let root: Root

### Enumerations

enum CommonKeyPathKind

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- PredicateExpression
- Sendable
- StandardPredicateExpression

  Conforms when `Root` conforms to `StandardPredicateExpression`, `Output` conforms to `Copyable`, and `Output` conforms to `Escapable`.

