

- StoreKit Test
- SKTestSession
-  simulatedError(forAPI:) 

Instance Method

# simulatedError(forAPI:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func simulatedError(forAPI api: API) async -> API.Failure? where API : FailableStoreKitAPI
```

## See Also

### Instance Methods

func buyProduct(identifier: Product.ID, options: Set&lt;Product.PurchaseOption>) async throws -> Transaction

func setSimulatedError&lt;API>(API.Failure?, forAPI: API) async throws

