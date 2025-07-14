

- Authentication Services
- ASAccountAuthenticationModificationViewController
-  extensionContext 

Instance Property

# extensionContext

The context your account authentication modification extension uses to provide information to the system.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var extensionContext: ASAccountAuthenticationModificationExtensionContext { get }
```

## Mentioned in 

Upgrading Account Security With an Account Authentication Modification Extension

## Discussion

Your extension uses the extension context to communicate with the system during the upgrade process.

