

- WebKit
-  WKWebExtension 

Class

# WKWebExtension

An object that encapsulates a web extension’s resources that the manifest file defines.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
class WKWebExtension
```

## Overview

This class reads and parses the `manifest.json` file along with the supporting resources like icons and localizations.

## Topics

### Classes

class Action

An object that encapsulates the properties for an individual web extension action.

class Command

An object that encapsulates the properties for an individual web extension command.

class DataRecord

An object that represents a record of stored data for a specific web extension context.

class MatchPattern

An object that represents a way to specify groups of URLs.

class MessagePort

An object that manages message-based communication with a web extension.

class TabConfiguration

An object that encapsulates configuration options for a tab in an extension.

class WindowConfiguration

An object that encapsulates configuration options for a window in an extension.

class Configuration

A WKWebExtensionController.Configuration object with which to initialize a web extension controller.

### Structures

struct DataType

Constants for specifying data types for a WKWebExtension.DataRecord.

struct Error

Constants that indicate errors in the WKWebExtension domain.

struct Permission

Constants for specifying permission in a WKWebExtensionContext.

struct TabChangedProperties

Constants the web extension controller and web extension context use to indicate tab changes.

### Enumerations

enum WindowState

Constants used by WKWebExtensionWindow to indicate possible states of a window.

enum WindowType

Constants used by WKWebExtensionWindow to indicate the type of a window.

### Initializers

convenience init(appExtensionBundle: Bundle) async throws

convenience init(resourceBaseURL: URL) async throws

### Instance Properties

var allRequestedMatchPatterns: Set&lt;WKWebExtension.MatchPattern>

The set of websites that the extension requires access to for injected content and for receiving messages from websites.

var defaultLocale: Locale?

The default locale for the extension.

var displayActionLabel: String?

The default localized extension action label.

var displayDescription: String?

The localized extension description.

var displayName: String?

The localized extension name.

var displayShortName: String?

The localized extension short name.

var displayVersion: String?

The localized extension display version.

var errors: [any Error]

An array of all errors that occurred during the processing of the extension.

var hasBackgroundContent: Bool

A Boolean value indicating whether the extension has background content that can run when needed.

var hasCommands: Bool

A Boolean value indicating whether the extension includes commands that users can invoke.

var hasContentModificationRules: Bool

A Boolean value indicating whether the extension includes rules used for content modification or blocking.

var hasInjectedContent: Bool

A Boolean value indicating whether the extension has script or stylesheet content that can be injected into webpages.

var hasOptionsPage: Bool

A Boolean value indicating whether the extension has an options page.

var hasOverrideNewTabPage: Bool

A Boolean value indicating whether the extension provides an alternative to the default new tab page.

var hasPersistentBackgroundContent: Bool

A Boolean value indicating whether the extension has background content that stays in memory as long as the extension is loaded.

var manifest: [String : Any]

The parsed manifest as a dictionary.

var manifestVersion: Double

The parsed manifest version, or `0` if there is no version specified in the manifest.

var optionalPermissionMatchPatterns: Set&lt;WKWebExtension.MatchPattern>

The set of websites that the extension may need access to for optional functionality.

var optionalPermissions: Set&lt;WKWebExtension.Permission>

The set of permissions that the extension may need for optional functionality.

var requestedPermissionMatchPatterns: Set&lt;WKWebExtension.MatchPattern>

The set of websites that the extension requires access to for its base functionality.

var requestedPermissions: Set&lt;WKWebExtension.Permission>

The set of permissions that the extension requires for its base functionality.

var version: String?

The extension version.

### Instance Methods

func actionIcon(for: CGSize) -> UIImage?

Returns the default action icon for the specified size.

func icon(for: CGSize) -> UIImage?

Returns the extension’s icon image for the specified size.

func supportsManifestVersion(Double) -> Bool

Checks if a manifest version is supported by the extension.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Web extensions

protocol WKWebExtensionTab

A protocol with methods that represent a tab to web extensions.

protocol WKWebExtensionWindow

A protocol with methods that represent a window to web extensions.

class WKWebExtensionContext

An object that represents the runtime environment for a web extension.

class WKWebExtensionController

An object that manages a set of loaded extension contexts.

protocol WKWebExtensionControllerDelegate

A group of methods you use to customize web extension interactions.

