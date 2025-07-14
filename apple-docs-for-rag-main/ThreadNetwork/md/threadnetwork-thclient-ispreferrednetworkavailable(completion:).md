

- ThreadNetwork
- THClient
-  isPreferredNetworkAvailable(completion:) 

Instance Method

# isPreferredNetworkAvailable(completion:)

Indicates whether a preferred network is available.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.0+visionOS 1.0+

``` source
func isPreferredNetworkAvailable(completion: @escaping (Bool) -> Void)
```

``` source
func isPreferredAvailable() async -> Bool
```

## Parameters 

`completion`  

The completion handler that returns the result of the preferred network status.

## Mentioned in 

Configuring a Border Router

Managing Thread network credentials

## Discussion

Concurrency note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func isPreferredAvailable() async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Call the method as follows:

```
func obtainPreferredAvailable() async -> (NSString?) {
    let client = THClient()
    var bIsPreferredAvailable:Bool?
    bIsPreferredAvailable = await client.isPreferredAvailable()
    let str = ((bIsPreferredAvailable == true) ? "true" : "false")
    return str as NSString;
}
```

## See Also

### Retrieving Credentials

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

func retrieveAllActiveCredentials((Set&lt;THCredentials>?, (any Error)?) -> Void)

Returns a set of the active credentials.

