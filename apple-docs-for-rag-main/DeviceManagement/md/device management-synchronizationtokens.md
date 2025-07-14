

- Device Management
-  SynchronizationTokens 

Object

# SynchronizationTokens

The server’s synchronization token.

Device Assignment ServicesVPP License Management

``` source
object SynchronizationTokens
```

## Properties

`DeclarationsToken`

`string`

 (Required) 

The synchronization token for declarations.

`Timestamp`

`date-time`

 (Required) 

The timestamp for the creation of the set of sync tokens. Clients use this to determine the most recent set of sync tokens when different sources provide the tokens. Use the format `YYYY-mm-ddTHH:MM:SSZ`.

## Mentioned in 

Integrating Declarative Management

