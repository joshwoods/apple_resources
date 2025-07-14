

- Network Extension
-  NEDNSProxyManager 

Class

# NEDNSProxyManager

An object to create and manage an DNS proxy provider’s configuration.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class NEDNSProxyManager
```

## Overview

A DNS proxy allows your app to intercept all DNS traffic generated on a device. You can use this capability to provide services like DNS traffic encryption, typically by redirecting DNS traffic to your own server. You usually do this in the context of managed devices, such as those owned by a school or an enterprise.

You create a DNS proxy as an app extension based on a custom subclass of the NEDNSProxyProvider class. You enable and configure this proxy from within your app using the singleton proxy manager instance provided by the shared() type method of the NEDNSProxyManager class. For example, for a proxy that performs a simple redirect, you can use the proxy manager to define and dynamically configure the destination IP address of the redirected traffic.

Instances of the proxy manager are thread safe.

Important

To use the NEDNSProxyManager class, you must enable the Network Extensions capability in Xcode and select the DNS Proxy capability. See Configure network extensions.

## Topics

### Managing the DNS proxy configuration

class func shared() -> NEDNSProxyManager

Returns a singleton DNS proxy manager instance.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Loads the current DNS proxy configuration from the caller’s DNS proxy preferences.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Saves the DNS proxy configuration in the caller’s DNS proxy preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Removes the DNS proxy configuration from the caller’s DNS proxy preferences.

### Accessing DNS proxy configuration properties

var isEnabled: Bool

The status of a DNS proxy.

var providerProtocol: NEDNSProxyProviderProtocol?

The provider-specific portion of the DNS proxy configuration.

var localizedDescription: String?

A description of the DNS proxy.

### Notifications

static let NEDNSProxyConfigurationDidChange: NSNotification.Name

A notification that is posted when the DNS proxy configuration changes.

### Errors

let NEDNSProxyErrorDomain: String

The DNS proxy error domain.

enum NEDNSProxyManagerError

The possible DNS proxy manager errors.

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

### Configuration

class NEDNSProxyProviderProtocol

Configuration parameters for a DNS proxy.

