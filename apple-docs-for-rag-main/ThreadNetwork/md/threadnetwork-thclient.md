

- ThreadNetwork
-  THClient 

Class

# THClient

A class that supports safely sharing Thread credentials between multiple clients.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+

``` source
class THClient
```

## Overview

Request credentials for either a specific Thread network or for the *preferred network* using THClient. The preferred network is the default Thread network chosen by the framework for a home.

The ThreadNetwork framework maintains a database of network credentials. The class allows clients to store, list, and delete credentials for a given network from the database.

Some methods in THClient use the *team ID*, a string that you store in your application’s `Info.plist`. The ThreadNetwork framework uses the team ID to preserve the privacy of the Thread network credentials across different clients. For example, credentials stored by one client can’t be deleted or modified by another client.

Important

Thread credentials give you the ability to add any device into the Thread network. Use this information responsibly.

## Topics

### Creating the Client

init()

Creates the client object.

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

func retrieveAllActiveCredentials((Set&lt;THCredentials>?, (any Error)?) -> Void)

Returns a set of the active credentials.

### Storing and Deleting Credentials

func deleteCredentials(forBorderAgent: Data, completion: ((any Error)?) -> Void)

Deletes Thread network credentials from the framework database for a Border Agent.

func storeCredentials(forBorderAgent: Data, activeOperationalDataSet: Data, completion: ((any Error)?) -> Void)

Stores Thread network credentials into the framework database that a Border Agent provides.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Managing clients and sharing credentials

com.apple.developer.networking.manage-thread-network-credentials

A Boolean value that indicates whether the app can use ThreadNetwork.

class THCredentials

A class that contains credentials for a Thread network.

