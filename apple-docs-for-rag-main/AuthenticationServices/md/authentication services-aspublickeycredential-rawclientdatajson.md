

- Authentication Services
- ASPublicKeyCredential
-  rawClientDataJSON 

Instance Property

# rawClientDataJSON

Raw data that contains a JSON-compatible encoding of the client data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var rawClientDataJSON: Data { get }
```

**Required**

## Discussion

This object acts as an input to the signing algorithm. It needs to be in JSON form for the relying party to verify the provided signature. The developer should ignore this value.

## See Also

### Getting the properties

var credentialID: Data

An identifier that the authenticator generates during registration to uniquely identify a specific credential.

**Required**

