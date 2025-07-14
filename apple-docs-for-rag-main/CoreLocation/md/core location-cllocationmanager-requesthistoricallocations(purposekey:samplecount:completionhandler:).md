

- Core Location
- CLLocationManager
-  requestHistoricalLocations(purposeKey:sampleCount:completionHandler:) 

Instance Method

# requestHistoricalLocations(purposeKey:sampleCount:completionHandler:)

watchOS 9.0+

``` source
func requestHistoricalLocations(
    purposeKey: String,
    sampleCount: Int,
    completionHandler handler: @escaping ([CLLocation], (any Error)?) -> Void
)
```

``` source
func historicalLocations(
    purposeKey: String,
    sampleCount: Int
) async throws -> [CLLocation]
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func historicalLocations(purposeKey: String, sampleCount: Int) async throws -> [CLLocation]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

