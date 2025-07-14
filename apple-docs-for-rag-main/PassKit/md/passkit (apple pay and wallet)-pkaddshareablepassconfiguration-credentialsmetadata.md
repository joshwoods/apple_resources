

- PassKit (Apple Pay and Wallet)
- PKAddShareablePassConfiguration
-  credentialsMetadata 

Instance Property

# credentialsMetadata

Information for a shareable pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+

``` source
var credentialsMetadata: [PKShareablePassMetadata] { get }
```

## See Also

### Creating a pass configuration

class func forPassMetaData([PKShareablePassMetadata], provisioningPolicyIdentifier: String, action: PKAddShareablePassConfigurationPrimaryAction, completion: (PKAddShareablePassConfiguration?, (any Error)?) -> Void)

Creates and error checks a new shareable pass-configuration object.

Deprecated

var primaryAction: PKAddShareablePassConfigurationPrimaryAction

The action that the system performs with the shareable pass.

var provisioningPolicyIdentifier: StringDeprecated

