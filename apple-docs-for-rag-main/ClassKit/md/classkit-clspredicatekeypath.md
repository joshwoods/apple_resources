

- ClassKit
-  CLSPredicateKeyPath 

Structure

# CLSPredicateKeyPath

The set of possible key paths you use to search for contexts.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
struct CLSPredicateKeyPath
```

## Discussion

Use these predicate key paths when constructing a predicate to send to the contexts(matching:completion:) method.

## Topics

### Predicate Key Paths

static let dateCreated: CLSPredicateKeyPath

The date on which the context was created.

static let identifier: CLSPredicateKeyPath

The context’s identifier.

static let parent: CLSPredicateKeyPath

The context’s direct ancestor in the context hierarchy.

static let title: CLSPredicateKeyPath

The human readable name of the context.

static let topic: CLSPredicateKeyPath

The context’s topic.

static let universalLinkURL: CLSPredicateKeyPath

The context’s universal URL link.

### Initializing a Predicate Key Path

init(String)

Initializes a predicate key path.

init(rawValue: String)

Initializes a predicate key path with the given value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Finding contexts that match criteria

func contexts(matchingIdentifierPath: [String], completion: ([CLSContext], (any Error)?) -> Void)

Fetches all the contexts along a given identifier path.

func contexts(matching: NSPredicate, completion: ([CLSContext], (any Error)?) -> Void)

Fetches all the contexts matching a predicate.

