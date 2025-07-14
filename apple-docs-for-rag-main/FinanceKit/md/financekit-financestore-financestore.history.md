

- FinanceKit
- FinanceStore
-  FinanceStore.History 

Structure

# FinanceStore.History

A structure the framework uses to collect and iterate over finance store model objects.

iOS 17.4+iPadOS 17.4+

``` source
struct History where Model : Identifiable
```

## Topics

### Structures

struct Iterator

The type that allows iteration over an array’s elements

### Instance Methods

func makeAsyncIterator() -> FinanceStore.History&lt;Model>.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence

typealias Element

An alias for the type that this asynchronous sequence holds.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence
- Sendable

