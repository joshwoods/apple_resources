

- ThreadNetwork
- THClient
-  retrieveCredentials(forExtendedPANID:completion:) 

Instance Method

# retrieveCredentials(forExtendedPANID:completion:)

Requests Thread credentials for an extended Personal Area Network (PAN) ID.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+

``` source
func retrieveCredentials(
    forExtendedPANID extendedPANID: Data,
    completion: @escaping (THCredentials?, (any Error)?) -> Void
)
```

``` source
func credentials(forExtendedPANID extendedPANID: Data) async throws -> THCredentials
```

## Parameters 

`extendedPANID`  

The extended PAN identifier.

`completion`  

The completion handler the framework calls when the credentials become available.

## Discussion

Concurrency note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func credentials(forExtendedPANID extendedPANID: Data) async throws -> THCredentials
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

When calling this method, an alert appears asking for user permission to access credentials.

Call the method as follows:

```
func obtainCredentials(xpanID: Data) async -> (cred: THCredentials? ,err: Error? ) {
    let client = THClient()
    var credential: THCredentials?
    var err:Error?
    do {
        credential = try await client.credentials(forExtendedPANID: xpanID as Data)
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

func retrieveAllCredentials((Set&lt;THCredentials>?, (any Error)?) -> Void)

Requests all Thread credentials from the framework.

func retrievePreferredCredentials((THCredentials?, (any Error)?) -> Void)

Requests Thread credentials for the preferred network.

func retrieveAllActiveCredentials((Set&lt;THCredentials>?, (any Error)?) -> Void)

Returns a set of the active credentials.

