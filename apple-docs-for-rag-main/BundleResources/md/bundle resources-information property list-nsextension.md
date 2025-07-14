

- Bundle Resources
- Information Property List
-  NSExtension 

Property List Key

# NSExtension

The properties of an app extension.

iOS 8.0+iPadOS 8.0+macOS 10.10+visionOS 1.0+

## Details 

Type  

object

## Topics

### Appearance and Presentation

NSExtensionActionWantsFullScreenPresentation

A Boolean value indicating whether the Action extension is presented in full screen.

NSExtensionMainStoryboard

The name of the app extension’s main storyboard file.

NSExtensionOverridesHostUIAppearance

A Boolean value indicating whether the app extension ignores appearance changes made by the host app.

NSExtensionPointIdentifier

The extension point that supports an app extension.

NSExtensionPrincipalClass

The custom class that implements an app extension’s primary view or functionality.

### Attributes

NSExtensionAttributes

Properties of an app extension.

### Authentication

ASAccountAuthenticationModificationPasswordGenerationRequirements

The rules the system satisfies when generating a strong password for your extension during an automatic upgrade.

ASAccountAuthenticationModificationSupportsStrongPasswordChange

A Boolean value that indicates whether the extension supports upgrading a user’s password to a strong password.

ASAccountAuthenticationModificationSupportsUpgradeToSignInWithApple

A Boolean value that indicates whether the extension supports upgrading from using password authentication to using Sign in with Apple.

### File Provider

NSExtensionFileProviderActions

The custom actions for a File Provider extension.

NSExtensionFileProviderDocumentGroup

The identifier of a shared container that can be accessed by a Document Picker extension and its associated File Provider extension.

**Name:** App group used for document storage

NSExtensionFileProviderSupportsEnumeration

A Boolean value that indicates whether a File Provider extension enumerates its content.

**Name:** File Provider supports Enumeration

NSExtensionFileProviderDownloadPipelineDepth

The per-domain limit of concurrent calls that a file provider extension can make to fetch data from remote storage.

NSExtensionFileProviderUploadPipelineDepth

The per-domain limit of concurrent calls that a file provider extension can make to upload data.

### Intents

IntentsSupported

The names of the intents that an extension supports.

### Professional Video Applications

ProExtensionAttributes

A dictionary that specifies the minimum size of the floating window in which Final Cut Pro hosts the extension view.

ProExtensionPrincipalClass

The name of the class with the principal implementation of your extension.

ProExtensionPrincipalViewControllerClass

The name of the principal view controller class of your extension.

ProExtensionUUID

A UUID string that uniquely identifies your extension to the Compressor app.

### SafariServices

SFSafariContentScript

The content scripts for a Safari extension.

SFSafariContextMenu

The context menu items for a Safari extension.

SFSafariStyleSheet

The style sheet for a Safari extension.

SFSafariToolbarItem

The items to add to the toolbar for a Safari extension.

SFSafariWebsiteAccess

The webpages a Safari extension can access.

## See Also

### Extensions and services

NSServices

The services provided by an app.

**Name:** Services

WKExtensionDelegateClassName

The name of your watchOS app’s extension delegate.

UIApplicationShortcutWidget

The bundle ID of the widget that’s available as a Home screen quick action in apps that have more than one widget.

**Name:** Home Screen Widget

