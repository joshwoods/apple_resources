

- ThreadNetwork
- THClient
-  checkPreferredNetwork(forActiveOperationalDataset:completion:) 

Instance Method

# checkPreferredNetwork(forActiveOperationalDataset:completion:)

Determines if the essential operating parameters match the preferred network’s parameters.

iOS 15.5+iPadOS 15.5+Mac Catalyst 15.5+macOS 13.0+visionOS 1.0+

``` source
func checkPreferredNetwork(
    forActiveOperationalDataset activeOperationalDataSet: Data,
    completion: @escaping (Bool) -> Void
)
```

``` source
func isPreferred(forActiveOperationalDataset activeOperationalDataSet: Data) async -> Bool
```

## Parameters 

`activeOperationalDataSet`  

The essential operating parameters to compare against the preferred network’s parameters.

`completion`  

The completion handler that returns the result of the comparison.

## Mentioned in 

Managing Thread network credentials

Configuring a Border Router

## Discussion

Concurrency note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Call the method as follows:

```
```

## See Also

### Retrieving Credentials

func isPreferredNetworkAvailable(completion: (Bool) -> Void)

Indicates whether a preferred network is available.

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

