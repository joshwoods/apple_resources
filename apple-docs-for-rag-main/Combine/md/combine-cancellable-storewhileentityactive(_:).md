

- Combine
- Cancellable
-  storeWhileEntityActive(\_:) 

Instance Method

# storeWhileEntityActive(\_:)

Retains the `Cancellable` as long as the entity is active (see `Entity.isActive`). If the entity is deactivated, the `Cancellable` is released.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func storeWhileEntityActive(_ entity: Entity)
```

## Discussion

This method does nothing if the entity is already inactive.

Internally, this method stores an `AnyCancellable` in a transient component of the entity. The component is removed when the *deactivate* event for this entity is received.

