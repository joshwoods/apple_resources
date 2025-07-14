

- Local Authentication
- LAContext
-  isCredentialSet(\_:) 

Instance Method

# isCredentialSet(\_:)

Returns a Boolean value indicating whether the specified credential type is set.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 3.0+

``` source
func isCredentialSet(_ type: LACredentialType) -> Bool
```

## Parameters 

`type`  

The type of the credential. For possible values, see LACredentialType

## Return Value

true if the credential is set, otherwise false.

## See Also

### Managing credentials

func setCredential(Data?, type: LACredentialType) -> Bool

Sets an application-provided credential to be used when evaluating authentication.

enum LACredentialType

The types of credentials to be used for authentication.

