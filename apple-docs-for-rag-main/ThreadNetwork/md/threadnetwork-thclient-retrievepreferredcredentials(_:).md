

- ThreadNetwork
- THClient
-  retrievePreferredCredentials(\_:) 

Instance Method

# retrievePreferredCredentials(\_:)

Requests Thread credentials for the preferred network.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+

``` source
func retrievePreferredCredentials(_ completion: @escaping (THCredentials?, (any Error)?) -> Void)
```

``` source
func preferredCredentials() async throws -> THCredentials
```

## Parameters 

`completion`  

The completion handler the framework calls when the credentials become available.

## Mentioned in 

Managing Thread network credentials

Configuring a Border Router

## Discussion

Concurrency note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func preferredCredentials() async throws -> THCredentials
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

When you call this method, an alert appears asking for user permission to access credentials.

Call the method as follows:

```
func obtainPreferredCredentials() async -> (cred: THCredentials? , err: Error? ) {
    let client = THClient()
    var credential: THCredentials?
    var err:Error?
    do {
        credential = try await client.preferredCredentials()
    } catch {
        err = error
    }
    return (credential, err)
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

func retrieveAllActiveCredentials((Set&lt;THCredentials>?, (any Error)?) -> Void)

Returns a set of the active credentials.

