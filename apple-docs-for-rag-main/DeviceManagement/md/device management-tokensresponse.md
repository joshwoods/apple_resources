

- Device Management
-  TokensResponse 

Object

# TokensResponse

The response object that contains the device token.

Device Assignment ServicesVPP License Management

``` source
object TokensResponse
```

## Properties

`SyncTokens`

SynchronizationTokens

 (Required) 

A dictionary of synchronization tokens that describes the state of different types of data on the server. The client uses these tokens to determine which endpoints it needs to use to fetch new or updated data on the server.

## Topics

### Supporting Objects

object SynchronizationTokens

The server’s synchronization token.

