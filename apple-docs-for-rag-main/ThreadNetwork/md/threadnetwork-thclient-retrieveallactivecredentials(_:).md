

- ThreadNetwork
- THClient
-  retrieveAllActiveCredentials(\_:) 

Instance Method

# retrieveAllActiveCredentials(\_:)

Returns a set of the active credentials.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.0+visionOS 1.0+

``` source
func retrieveAllActiveCredentials(_ completion: @escaping (Set?, (any Error)?) -> Void)
```

``` source
func allActiveCredentials() async throws -> Set
```

## Parameters 

`completion`  

The completion handler the framework calls when the active credentials become available.

## Mentioned in 

Managing Thread network credentials

## Discussion

Concurrency note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func allActiveCredentials() async throws -> Set
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Call the method as follows:

```
func obtainAllActiveCredentials() async -> (Set?, Error?) {
    let client = THClient()
    var credentials: Set?
    var err:Error?
    do {
        credentials = try await client.allActiveCredentials()
    } catch {
        err = error
    }
    return (credentials, err)
}
```

## See Also

### Retrieving Credentials

func isPreferredNetworkAvailable(completion: (Bool) -> Void)

Indicates whether a preferred network is available.

func checkPreferredNetwork(forActiveOperationalDataset: Data, completion: (Bool) -> Void)

Determines if the essential operating parameters match the preferred network’s parameters.

func retrieveCredentials(forBorderAgent: Data, completion: (THCredentials?, (any Error)?) -> Void)

Requests Thread credentials for a Border Agent.

func retrieveCredentials(forExtendedPANID: Data, completion: (THCredentials?, (any Error)?) -> Void)

Requests Thread credentials for an extended Personal Area Network (PAN) ID.

func retrieveAllCredentials((Set&lt;THCredentials>?, (any Error)?) -> Void)

Requests all Thread credentials from the framework.

func retrievePreferredCredentials((THCredentials?, (any Error)?) -> Void)

Requests Thread credentials for the preferred network.

