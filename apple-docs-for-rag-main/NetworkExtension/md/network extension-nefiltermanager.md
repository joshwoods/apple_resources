

- Network Extension
-  NEFilterManager 

Class

# NEFilterManager

An object to create and manage a content filter’s configuration.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class NEFilterManager
```

## Overview

Each app is allowed to create a single filter configuration. The NEFilterManager class has a class method (shared()) that provides access to a single NEFilterManager instance. This single instance corresponds to a single filter configuration.

The filter configuration is stored in the Network Extension preferences which are managed by the Network Extension framework. The filter configuration must be explicitly loaded into memory from the Network Extension preferences before it can be used, and any changes must be explicitly saved to the Network Extension preferences before taking effect on the system.

Important

In product builds for distribution, Network Content Filter configurations can be created only on supervised devices. During development and testing you can temporarily override this restriction by signing your build with the `get-task-allow` entitlement.

Important

To use the NEFilterManager class, you must enable the Network Extensions capability in Xcode and select the Content Filter capability. See Configure network extensions.

### Profile Configuration

Filter configurations are created using configuration profiles. See WebContentFilter for more information. To specify that a filter configuration created via a profile payload is associated with a particular app (and therefore allow the app to use `NEFilterManager` to manage the configuration), the app’s bundle identifier must be set as the value of the `PluginBundleID` field in the profile payload.

### Filter Provider Extensions

Apps that use `NEFilterManager` are required to contain two Filter Provider extensions that together perform the task of examining network content and making pass and block decisions. See the NEFilterControlProvider and NEFilterDataProvider classes for more details about these extensions.

## Topics

### Managing the filter configuration

class func shared() -> NEFilterManager

Access the single instance of `NEFilterManager`.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load the filter configuration from the Network Extension preferences.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Save the filter configuration in the Network Extension preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Remove the filter configuration from the Network Extension preferences.

### Accessing filter configuration properties

var isEnabled: Bool

A Boolean used to toggle the enabled state of the filter.

var providerConfiguration: NEFilterProviderConfiguration?

A NEFilterProviderConfiguration object containing the filter configuration settings.

var localizedDescription: String?

A string containing a description of the filter configuration.

### Prioritizing filters

var grade: NEFilterManager.Grade

The grade of the filter, which determines when it acts relative to other filters.

enum Grade

A type for the grade or priority of the filter.

### Errors

let NEFilterErrorDomain: String

The domain for errors resulting from calls to the filter manager.

enum NEFilterManagerError

Error codes specific to filter managers.

### Notifications

static let NEFilterConfigurationDidChange: NSNotification.Name

Posted after the filter configuration stored in the Network Extension preferences changes.

### Instance Properties

var disableEncryptedDNSSettings: Bool

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

## See Also

### Filter configuration

class NEFilterProviderConfiguration

Configuration parameters for a content filter.

