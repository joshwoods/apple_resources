

- SecureElementCredential
- CredentialSession
-  provisionCredential(configurationUUID:name:) 

Instance Method

# provisionCredential(configurationUUID:name:)

Creates a credential in the Secure Element.

iOS 18.1+iPadOS 18.1+

``` source
func provisionCredential(
    configurationUUID: UUID,
    name: String
) async throws -> CredentialSession.Credential
```

## Parameters 

`configurationUUID`  

A UUID corresponding to an applet bundle configured on the Apple Business Register portal. The system uses the corresponding applet bundle to provision the instance associated with the created credential. The UUID is opaque to the device.

`name`  

A friendly name assigned for ease of identification the provisioned credential. The name is opaque to the device.

## Return Value

A CredentialSession.Credential, initialized with the CredentialSession.Credential.State.installationPending state.

## Mentioned in 

Accessing and using secure element credentials

## Discussion

This method installs into the Secure Element an applet bundle that you’ve submitted through the Apple Business Register portal.

## See Also

### Managing a credential

func deleteCredential(CredentialSession.Credential) async throws

Deletes a credential on the Secure Element.

