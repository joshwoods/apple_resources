

- PassKit (Apple Pay and Wallet)
- PKAddShareablePassConfiguration
-  primaryAction 

Instance Property

# primaryAction

The action that the system performs with the shareable pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+

``` source
var primaryAction: PKAddShareablePassConfigurationPrimaryAction { get }
```

## See Also

### Creating a pass configuration

class func forPassMetaData([PKShareablePassMetadata], provisioningPolicyIdentifier: String, action: PKAddShareablePassConfigurationPrimaryAction, completion: (PKAddShareablePassConfiguration?, (any Error)?) -> Void)

Creates and error checks a new shareable pass-configuration object.

Deprecated

var credentialsMetadata: [PKShareablePassMetadata]

Information for a shareable pass.

var provisioningPolicyIdentifier: StringDeprecated

