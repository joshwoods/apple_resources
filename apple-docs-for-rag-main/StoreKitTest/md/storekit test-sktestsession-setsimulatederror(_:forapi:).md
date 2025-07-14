

- StoreKit Test
- SKTestSession
-  setSimulatedError(\_:forAPI:) 

Instance Method

# setSimulatedError(\_:forAPI:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func setSimulatedError(
    _ error: API.Failure?,
    forAPI api: API
) async throws where API : FailableStoreKitAPI
```

## See Also

### Instance Methods

func buyProduct(identifier: Product.ID, options: Set&lt;Product.PurchaseOption>) async throws -> Transaction

func simulatedError&lt;API>(forAPI: API) async -> API.Failure?

