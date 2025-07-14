

- StoreKit Test
- SKTestSession
-  buyProduct(identifier:options:) 

Instance Method

# buyProduct(identifier:options:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@discardableResult
func buyProduct(
    identifier: Product.ID,
    options: Set = []
) async throws -> Transaction
```

## See Also

### Instance Methods

func setSimulatedError&lt;API>(API.Failure?, forAPI: API) async throws

func simulatedError&lt;API>(forAPI: API) async -> API.Failure?

