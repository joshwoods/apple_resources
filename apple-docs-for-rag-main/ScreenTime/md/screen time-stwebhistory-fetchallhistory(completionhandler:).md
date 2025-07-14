

- Screen Time
- STWebHistory
-  fetchAllHistory(completionHandler:) 

Instance Method

# fetchAllHistory(completionHandler:)

Fetches all web history associated with the bundle identifier and profile identifier you specified during initialization.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+

``` source
func fetchAllHistory(completionHandler: @escaping (Set?, (any Error)?) -> Void)
```

``` source
func fetchAllHistory() async throws -> Set
```

