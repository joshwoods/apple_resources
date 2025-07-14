

- FinanceKit
- FinanceStore
- FinanceStore.History
-  FinanceStore.History.Iterator 

Structure

# FinanceStore.History.Iterator

The type that allows iteration over an array’s elements

iOS 17.4+iPadOS 17.4+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() async throws -> FinanceStore.Changes&lt;Model>?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

