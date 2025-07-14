

- Combine
- Just
-  max(by:) 

Instance Method

# max(by:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func max(by areInIncreasingOrder: (Output, Output) -> Bool) -> Just
```

## See Also

### Applying Mathematical Operations on Elements

func count() -> Just&lt;Int>

func max() -> Just&lt;Output>

func tryMax(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the maximum value received from the upstream publisher, using the provided error-throwing closure to order the items.

func min() -> Just&lt;Output>

func min(by: (Output, Output) -> Bool) -> Just&lt;Output>

func tryMin(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the minimum value received from the upstream publisher, using the provided error-throwing closure to order the items.

