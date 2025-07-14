

- Local Authentication
- LAContext
-  setCredential(\_:type:) 

Instance Method

# setCredential(\_:type:)

Sets an application-provided credential to be used when evaluating authentication.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 3.0+

``` source
func setCredential(
    _ credential: Data?,
    type: LACredentialType
) -> Bool
```

## Parameters 

`credential`  

The credential to be used when evaluating the authentication context.

Setting this parameter to `nil` removes any existing credential of the specified type.

`type`  

The type of the specified credential. For possible values, see LACredentialType.

## Return Value

true if the credential was set, otherwise false.

## See Also

### Managing credentials

func isCredentialSet(LACredentialType) -> Bool

Returns a Boolean value indicating whether the specified credential type is set.

enum LACredentialType

The types of credentials to be used for authentication.

