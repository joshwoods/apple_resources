

- PassKit (Apple Pay and Wallet)
- PKAddShareablePassConfiguration
-  forPassMetaData(\_:provisioningPolicyIdentifier:action:completion:) Deprecated

Type Method

# forPassMetaData(\_:provisioningPolicyIdentifier:action:completion:)

Creates and error checks a new shareable pass-configuration object.

iOS 14.0–16.0DeprecatediPadOS 14.0–16.0DeprecatedMac Catalyst 14.0–16.0DeprecatedmacOSvisionOS 1.0–1.0Deprecated

``` source
class func forPassMetaData(
    _ passMetadata: [PKShareablePassMetadata],
    provisioningPolicyIdentifier: String,
    action: PKAddShareablePassConfigurationPrimaryAction,
    completion: @escaping (PKAddShareablePassConfiguration?, (any Error)?) -> Void
)
```

``` source
class func forPassMetaData(
    _ passMetadata: [PKShareablePassMetadata],
    provisioningPolicyIdentifier: String,
    action: PKAddShareablePassConfigurationPrimaryAction
) async throws -> PKAddShareablePassConfiguration
```

Deprecated

Use configurationForPassMetadata:primaryAction:completion:

## Parameters 

`passMetadata`  

`provisioningPolicyIdentifier`  

`action`  

The action that the system performs with the shareable pass.

`completion`  

A completion handler that returns the shareable pass configuration or an error. This handler takes the following parameters:

`shareableCredentialConfiguration`  
A PKAddShareablePassConfiguration that contains the shareable pass configuration, or `nil` if an error occurred.

`error`  
An NSError that contains the error, or `nil` if no error occurred.

## See Also

### Creating a pass configuration

var primaryAction: PKAddShareablePassConfigurationPrimaryAction

The action that the system performs with the shareable pass.

var credentialsMetadata: [PKShareablePassMetadata]

Information for a shareable pass.

var provisioningPolicyIdentifier: StringDeprecated

