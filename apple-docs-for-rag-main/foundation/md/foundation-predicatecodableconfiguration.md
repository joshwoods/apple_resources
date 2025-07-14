

- Foundation
-  PredicateCodableConfiguration 

Structure

# PredicateCodableConfiguration

A specification of the expected types and key paths found in an archived predicate.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct PredicateCodableConfiguration
```

## Overview

Use this configuration when encoding and decoding a predicate to restrict what that predicate can contain. If a predicate contains data types or keypaths that aren’t allowed by the configuration, the encoding or decoding process throws an error.

```
var configuration = PredicateCodableConfiguration.standardConfiguration
configuration.allowType(Message.self, identifier: "MyApp.Message")
configuration.allowType(Person.self, identifier: "MyApp.Person")
configuration.allowKeyPath(\Message.sender, identifier: "MyApp.Message.sender")
configuration.allowKeyPath(\Person.firstName, identifier: "MyApp.Person.firstName")
configuration.allowKeyPath(\Person.lastName, identifier: "MyApp.Person.lastName")

struct MyRequest: Codable {
    let predicate: Predicate

    func encode(to encoder: Encoder) throws {
        var container = encoder.container(keyedBy: CodingKeys.self)
        try container.encode(predicate, forKey: .predicate, configuration: configuration)
    }

    init(from decoder: Decoder) throws {
        let container = try decoder.container(keyedBy: CodingKeys.self)
        predicate = try container.decode(Predicate.self, forKey: .predicate, configuration: configuration)
    }
}
```

## Topics

### Creating a configuration

init()

static let standardConfiguration: PredicateCodableConfiguration

### Allowing types and key paths

func allow(PredicateCodableConfiguration)

func allowKeyPathsForPropertiesProvided&lt;T>(by: T.Type, recursive: Bool)

func allowPartialType(any Any.Type, identifier: String)

func allowType(any Any.Type, identifier: String?)

### Disallowing types and key paths

func disallowKeyPathsForPropertiesProvided&lt;T>(by: T.Type, recursive: Bool)

func disallowPartialType(any Any.Type)

func disallowType(any Any.Type)

### Instance Methods

func allowKeyPath(any AnyKeyPath &amp; Sendable, identifier: String)

func disallowKeyPath(any AnyKeyPath &amp; Sendable)

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Sendable

## See Also

### Filltering

struct Predicate

A logical condition used to test a set of input values for searching or filtering.

struct PredicateError

An error thrown while evaluating a predicate.

protocol PredicateCodableKeyPathProviding

A type that provides the expected key paths found in an archived predicate.

protocol PredicateExpression

A component expression that makes up part of a predicate.

protocol StandardPredicateExpression

A component expression that makes up part of a predicate, and that’s supported by the standard predicate type.

enum PredicateExpressions

The expressions that make up a predicate.

struct PredicateBindings

A mapping from a predicates’s input variables to their values.

class NSPredicate

A definition of logical conditions for constraining a search for a fetch or for in-memory filtering.

class NSExpression

An expression for use in a comparison predicate.

class NSComparisonPredicate

A specialized predicate for comparing expressions.

class NSCompoundPredicate

A specialized predicate that evaluates logical combinations of other predicates.

