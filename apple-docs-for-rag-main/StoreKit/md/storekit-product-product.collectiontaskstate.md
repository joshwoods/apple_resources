

- StoreKit
- Product
-  Product.CollectionTaskState 

Enumeration

# Product.CollectionTaskState

The state of a task that loads a collection of products in the background.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum CollectionTaskState
```

## Topics

### Collection task states

case loading

The task is loading the collection in the background.

case success([Product], unavailable: [Product.ID])

The task completed loading the collection.

case failure(any Error)

The task failed with an error.

### Instance Properties

var products: [Product]?

An array of available products if the task was successful.

## Relationships

### Conforms To

- Sendable

## See Also

### Loading products

enum TaskState

The state of a task that loads a product in the background.

