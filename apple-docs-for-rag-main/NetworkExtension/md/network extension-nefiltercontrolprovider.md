

- Network Extension
-  NEFilterControlProvider 

Class

# NEFilterControlProvider

The principal class for a filter control provider extension.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class NEFilterControlProvider
```

## Overview

The Filter Control Provider’s primary responsibility is to provide information to the associated Filter Data Provider so that it can perform its task of accurately filtering network content. There are several ways in which the Filter Control Provider provides data to the associated Filter Data Provider:

- By writing information to disk. For example, the Filter Control Provider can maintain a database of filtering rules on disk in a location where the Filter Data Provider can read from the database.

- By defining a dictionary that maps keys to sets of customization parameters to be used when generating the block page. The Filter Data Provider gives the system the key for the desired customization parameters, and the system uses that key to get the customization parameters from the Filter Control Provider and generate the customized block page.

- By defining a dictionary that maps keys to strings to be appended to URLs. The Filter Data Provider gives the system the key for the string to be appended, and the system uses that key to get the string to be appended from the Filter Control Provider and appends the string to the URL.

Important

To use the NEFilterControlProvider class, you must enable the Network Extensions capability in Xcode and select the Content Filter capability. See Configure network extensions.

### Creating a Filter Control Provider Extension

Filter Control Providers run as App Extensions for the `com.apple.networkextension.filter-control` extension point.

To create a Filter Control Provider extension, first create a new App Extension target in your project.

For an example of an Xcode build target for this app extension, see the SimpleTunnel: Customized Networking Using the NetworkExtension Framework sample code project.

Once you have a Filter Control Provider extension target, create a sub-class of `NEFilterControlProvider`. Then, set the `NSExtensionPrincipalClass` key in the the extension’s `Info.plist` to the name of your subclass.

If it is not already, set the `NSExtensionPointIdentifier` key in the extension’s `Info.plist` to `com.apple.networkextension.filter-control`.

Here is an example of the `NSExtension` dictionary in a Filter Control Provider extension’s `Info.plist`:

```
NSExtension

    NSExtensionPointIdentifier
    com.apple.networkextension.filter-control
    NSExtensionPrincipalClass
    MyCustomFilterControlProvider

```

Finally, add your Filter Control Provider extension target to your app’s Embed App Extensions build phase.

## Topics

### Handling requests for new rules

func handleNewFlow(NEFilterFlow, completionHandler: (NEFilterControlVerdict) -> Void)

Handle a request for new filtering rules.

func notifyRulesChanged()

Notify the Filter Data Provider that the filtering rules have changed on disk.

### Handling remediation

func handleRemediation(for: NEFilterFlow, completionHandler: (NEFilterControlVerdict) -> Void)

Handle a request for remediation from the user.

var remediationMap: [String : [String : NSObject]]?

A dictionary containing sets of strings used to customize the remediation portion of the block page.

let NEFilterProviderRemediationMapRemediationButtonTexts: String

A key in the remediationMap dictionary. The value of this key should be set to a dictionary that maps button text string identifiers to the text to display for the remediation URL link in the block page. The button text string identifiers are defined by the Filter Control Provider app extension.

let NEFilterProviderRemediationMapRemediationURLs: String

A key in the remediationMap dictionary. The value of this key should be set to a dictionary that maps URL identifiers to remediation URLs to be inserted into the block page. The URL identifiers are defined by the Filter Control Provider app extension.

var NEFilterProviderRemediationURLFlowURL: String

This string will be replaced with the full URL of the flow.

var NEFilterProviderRemediationURLFlowURLHostname: String

This string will be replaced with the hostname portion of the flow’s URL.

var NEFilterProviderRemediationURLOrganization: String

This string will be replaced with the value of the organization property set in the filter configuration.

var NEFilterProviderRemediationURLUsername: String

This string will be replaced with the value of the username property set in the filter configuration.

var urlAppendStringMap: [String : String]?

A dictionary containing strings to be appended to URLs.

## Relationships

### Inherits From

- NEFilterProvider

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Data and control providers

class NEFilterDataProvider

The principal class for a filter data provider extension.

class NEFilterPacketProvider

A filter provider that evaluates network packets and decides whether to block, allow, or delay the packets.

class NEFilterProvider

An abstract base class shared by content filters.

