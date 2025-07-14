

- Screen Time
- STWebHistory
-  fetchHistory(during:completionHandler:) 

Instance Method

# fetchHistory(during:completionHandler:)

Fetches web history that occurred during the date interval you specify.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+

``` source
func fetchHistory(
    during interval: DateInterval,
    completionHandler: @escaping (Set?, (any Error)?) -> Void
)
```

``` source
func fetchHistory(during interval: DateInterval) async throws -> Set
```

## Parameters 

`interval`  

The date interval of web history you want to fetch.

