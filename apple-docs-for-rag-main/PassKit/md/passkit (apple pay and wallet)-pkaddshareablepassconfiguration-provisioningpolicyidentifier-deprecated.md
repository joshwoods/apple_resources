

- PassKit (Apple Pay and Wallet)
- PKAddShareablePassConfiguration
-  provisioningPolicyIdentifier Deprecated

Instance Property

# provisioningPolicyIdentifier

iOS 14.0–16.0DeprecatediPadOS 14.0–16.0DeprecatedMac Catalyst 14.0–16.0DeprecatedmacOSvisionOS 1.0–1.0Deprecated

``` source
var provisioningPolicyIdentifier: String { get }
```

Deprecated

provisioningPolicyIdentifier has been deprecated. You can stop setting this property in the init with no repercussions.

## See Also

### Creating a pass configuration

class func forPassMetaData([PKShareablePassMetadata], provisioningPolicyIdentifier: String, action: PKAddShareablePassConfigurationPrimaryAction, completion: (PKAddShareablePassConfiguration?, (any Error)?) -> Void)

Creates and error checks a new shareable pass-configuration object.

Deprecated

var primaryAction: PKAddShareablePassConfigurationPrimaryAction

The action that the system performs with the shareable pass.

var credentialsMetadata: [PKShareablePassMetadata]

Information for a shareable pass.

