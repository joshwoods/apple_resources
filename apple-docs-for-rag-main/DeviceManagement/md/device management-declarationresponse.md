

- Device Management
-  DeclarationResponse 

Object

# DeclarationResponse

The details of a declaration, including its type and payload.

Device Assignment ServicesVPP License Management

``` source
object DeclarationResponse
```

## Properties

`Identifier`

`string`

 (Required) 

The unique identifier for this declaration.

`Payload`

DeclarationResponse.DeclarationPayload

 (Required) 

The payload that describes the declaration.

`ServerToken`

`string`

 (Required) 

A token that the server generates and the client treats as an opaque token. The client uses this token to determine if the payload in this response is different from the payload it already has. Servers compute the token over the entire declaration content to ensure the value always changes whenever there’s any change to the content.

`Type`

`string`

 (Required) 

The declaration’s type.

## Topics

### Supporting Objects

object DeclarationResponse.DeclarationPayload

The dictionary that contains the keys and values for a declaration payload.

