

- StoreKit
-  EntitlementTaskState 

Enumeration

# EntitlementTaskState

The state of an entitlement task.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum EntitlementTaskState
```

## Overview

To get an entitlement task state, use currentEntitlementTask(for:priority:action:) or subscriptionStatusTask(for:priority:action:) on a View.

## Topics

### Getting the task state

case loading

The task is loading the entitlement in the background.

case success(Value)

The task successfully loaded the entitlement.

case failure(any Error)

The task failed to load the entitlement, with an error.

### Getting the transaction with the entitlement

var transaction: VerificationResult&lt;Transaction>?

The transaction value if the task is successful.

var value: Value?

The entitlement value if the task is successful.

### Helper methods

func flatMap&lt;NewValue>((Value) throws -> EntitlementTaskState&lt;NewValue>) rethrows -> EntitlementTaskState&lt;NewValue>

Returns a new state, mapping the entitlement value if successful.

func flatMap&lt;NewValue>((Value) async throws -> EntitlementTaskState&lt;NewValue>) async rethrows -> EntitlementTaskState&lt;NewValue>

Returns a new state, mapping the entitlement value if successful.

func map&lt;NewValue>((Value) throws -> NewValue) rethrows -> EntitlementTaskState&lt;NewValue>

Returns a new state, mapping the entitlement value if successful.

func map&lt;NewValue>((Value) async throws -> NewValue) async rethrows -> EntitlementTaskState&lt;NewValue>

Returns a new state, mapping the entitlement value if successful.

## Relationships

### Conforms To

- Sendable

## See Also

### Loading StoreKit data

nonisolated func storeProductTask(for id: Product.ID, priority: TaskPriority = .medium, action: @escaping (Product.TaskState) async -> ()) -> some View 

Declares the view as dependent on an In-App Purchase product and returns a modified view.

nonisolated func storeProductsTask(for ids: some Collection&lt;String> &amp; Equatable &amp; Sendable, priority: TaskPriority = .medium, action: @escaping (Product.CollectionTaskState) async -> ()) -> some View 

Declares the view as dependent on a collection of In-App Purchase products and returns a modified view.

nonisolated func currentEntitlementTask(for productID: String, priority: TaskPriority = .medium, action: @escaping (EntitlementTaskState&lt;VerificationResult&lt;Transaction>?>) async -> ()) -> some View 

Declares the view as dependent on the entitlement of an In-App Purchase product, and returns a modified view.

nonisolated func subscriptionStatusTask(for groupID: String, priority: TaskPriority = .medium, action: @escaping (EntitlementTaskState&lt;[Product.SubscriptionInfo.Status]>) async -> ()) -> some View 

Declares the view as dependent on the status of an auto-renewable subscription group, and returns a modified view.

enum CollectionTaskState

The state of a task that loads a collection of products in the background.

enum TaskState

The state of a task that loads a product in the background.

