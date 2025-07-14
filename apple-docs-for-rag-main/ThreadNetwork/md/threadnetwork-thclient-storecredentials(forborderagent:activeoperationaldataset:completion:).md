

- ThreadNetwork
- THClient
-  storeCredentials(forBorderAgent:activeOperationalDataSet:completion:) 

Instance Method

# storeCredentials(forBorderAgent:activeOperationalDataSet:completion:)

Stores Thread network credentials into the framework database that a Border Agent provides.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+

``` source
func storeCredentials(
    forBorderAgent borderAgentID: Data,
    activeOperationalDataSet: Data,
    completion: @escaping ((any Error)?) -> Void
)
```

``` source
func storeCredentials(
    forBorderAgent borderAgentID: Data,
    activeOperationalDataSet: Data
) async throws
```

## Parameters 

`borderAgentID`  

The identifer of an active Thread network Border Agent.

`activeOperationalDataSet`  

The essential operational parameters for the Thread network.

`completion`  

The completion handler the framework calls after storing the credentials.

## Mentioned in 

Managing Thread network credentials

Configuring a Border Router

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func storeCredentials(forBorderAgent borderAgentID: Data, activeOperationalDataSet: Data) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The Border Agent is the software component running in the Border Router responsible for advertising itself in the Wi-Fi or Ethernet network.

The framework only stores credentials if it can find an mDNS record for the Border Agent that contains the specified Border Agent identifier.

Call the method as follows:

```
func saveCredentials(borderAgentID: Data, activeOperationalDataSet: Data) async -> (Error?) {
    let client = THClient()
    var err:Error?
    do {
        err = try await client.storeCredentials(forBorderAgent: borderAgentID, activeOperationalDataSet: activeOperationalDataSet) as? Error
    } catch {
        err = error
    }
    return (err)
}
```

## See Also

### Storing and Deleting Credentials

func deleteCredentials(forBorderAgent: Data, completion: ((any Error)?) -> Void)

Deletes Thread network credentials from the framework database for a Border Agent.

