

- StoreKit
- Product
-  Product.TaskState 

Enumeration

# Product.TaskState

The state of a task that loads a product in the background.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum TaskState
```

## Topics

### Task states

case loading

The task is loading the product in the background.

case success(Product)

The task successfully loaded the product.

case unavailable

The product is unavailable in the current storefront.

case failure(any Error)

The task failed with an error.

### Instance Properties

var product: Product?

The product value if the task was successful.

## Relationships

### Conforms To

- Sendable

## See Also

### Loading products

enum CollectionTaskState

The state of a task that loads a collection of products in the background.

