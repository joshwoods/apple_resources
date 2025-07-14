

- ThreadNetwork
- THClient
-  retrieveAllCredentials(\_:) 

Instance Method

# retrieveAllCredentials(\_:)

Requests all Thread credentials from the framework.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+

``` source
func retrieveAllCredentials(_ completion: @escaping (Set?, (any Error)?) -> Void)
```

``` source
func allCredentials() async throws -> Set
```

## Parameters 

`completion`  

The completion handler the framework calls when the credentials become available.

## Mentioned in 

Managing Thread network credentials

## Discussion

Concurrency note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func allCredentials() async throws -> Set
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The framework identifies the developer by the team ID. When calling this method, you receive credentials for your team ID only.

Call the method as follows:

```
func obtainAllCredentials() async -> (Set?, Error?) {
    let client = THClient()
    var credentials: Set?
    var err:Error?
    do {
        credentials = try await client.allCredentials()
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

func retrievePreferredCredentials((THCredentials?, (any Error)?) -> Void)

Requests Thread credentials for the preferred network.

func retrieveAllActiveCredentials((Set&lt;THCredentials>?, (any Error)?) -> Void)

Returns a set of the active credentials.

