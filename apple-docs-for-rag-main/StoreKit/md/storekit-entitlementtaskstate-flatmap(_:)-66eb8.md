

- StoreKit
- EntitlementTaskState
-  flatMap(\_:) 

Instance Method

# flatMap(\_:)

Returns a new state, mapping the entitlement value if successful.

StoreKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func flatMap(_ transform: (Value) async throws -> EntitlementTaskState) async rethrows -> EntitlementTaskState
```

## See Also

### Helper methods

func flatMap&lt;NewValue>((Value) throws -> EntitlementTaskState&lt;NewValue>) rethrows -> EntitlementTaskState&lt;NewValue>

Returns a new state, mapping the entitlement value if successful.

func map&lt;NewValue>((Value) throws -> NewValue) rethrows -> EntitlementTaskState&lt;NewValue>

Returns a new state, mapping the entitlement value if successful.

func map&lt;NewValue>((Value) async throws -> NewValue) async rethrows -> EntitlementTaskState&lt;NewValue>

Returns a new state, mapping the entitlement value if successful.

