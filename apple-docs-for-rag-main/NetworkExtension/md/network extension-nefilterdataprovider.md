

- Network Extension
-  NEFilterDataProvider 

Class

# NEFilterDataProvider

The principal class for a filter data provider extension.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class NEFilterDataProvider
```

## Overview

Network content is delivered to the Filter Data Provider in the form of NEFilterFlow objects. Each NEFilterFlow object corresponds to a network connection opened by an application running on the device. The Filter Data Provider can choose to pass or block the data when it receives a new flow, or it can ask the system to see more of the flow’s data in either the outbound or inbound direction before making a pass or block decision.

In addition to passing or blocking network data, the Filter Data Provider can tell the system that it needs more information before it can make a decision about a particular flow of data. The system will then ask the Filter Control Provider to update the current set of rules and place them in a location on disk that is readable from the Filter Data Provider extension.

When a NEFilterFlow object is originated from a WebKit browser object, the Filter Data Provider can affect the user experience in the following ways:

- If the Filter Data Provider chooses to block the web page, then a special “block” page is displayed in the WebKit browser object informing the user that their attempt to access the content was blocked. The Filter Data Provider can choose to add a link to this block page, giving the user the option of requesting access to the content.

- If the Filter Data Provider chooses to allow the web page, then it can also specify that a string be appended to the web page URL. This allows the Filter Data Provider to direct the WebKit browser object to a “safe” version of the web page.

To protect the user’s privacy, the Filter Data Provider extension sandbox prevents the extension from moving network content outside of its address space.

Important

To use the handleNewFlow(_:) method, you must enable the Network Extensions capability in Xcode and select the Content Filter capability. See Configure network extensions.

### Creating a Filter Data Provider Extension

Filter Data Providers run as App Extensions for the `com.apple.networkextension.filter-data` extension point.

To create a Filter Data Provider extension, first create a new App Extension target in your project.

For an example of an Xcode build target for this app extension, see the SimpleTunnel: Customized Networking Using the NetworkExtension Framework sample code project.

Once you have a Filter Data Provider extension target, create a subclass of `NEFilterDataProvider`. Then set the `NSExtensionPrincipalClass` key in the the extension’s `Info.plist` to the name of your subclass.

If it is not done already, set the `NSExtensionPointIdentifier` key in the extension’s `Info.plist` to `com.apple.networkextension.filter-data`.

Here is an example of the `NSExtension` dictionary in a Filter Data Provider extension’s `Info.plist`:

```
NSExtension

    NSExtensionPointIdentifier
    com.apple.networkextension.filter-data
    NSExtensionPrincipalClass
    MyCustomFilterDataProvider

```

Finally, add your Filter Data Provider extension target to your app’s Embed App Extensions build phase.

### Subclassing Notes

To create a Filter Data Provider extension, you must first create a subclass of `NEFilterDataProvider` and override the methods listed below.

#### Methods to Override

- handleNewFlow(_:)

- handleInboundData(from:readBytesStartOffset:readBytes:)

- handleOutboundData(from:readBytesStartOffset:readBytes:)

- handleInboundDataComplete(for:)

- handleOutboundDataComplete(for:)

- handleRemediation(for:)

- handleRulesChanged()

## Topics

### Filtering network content

func handleNewFlow(NEFilterFlow) -> NEFilterNewFlowVerdict

Make a filtering decision for a newly-created flow of network content.

func handleInboundData(from: NEFilterFlow, readBytesStartOffset: Int, readBytes: Data) -> NEFilterDataVerdict

Make a filtering decision about a chunk of inbound data.

enum NEFilterDataAttribute

Attribute flags that describe the data handled by a filter.

func handleOutboundData(from: NEFilterFlow, readBytesStartOffset: Int, readBytes: Data) -> NEFilterDataVerdict

Make a filtering decision about a chunk of outbound data.

func handleInboundDataComplete(for: NEFilterFlow) -> NEFilterDataVerdict

Make a filtering decision after seeing all of the inbound data for a flow.

func handleOutboundDataComplete(for: NEFilterFlow) -> NEFilterDataVerdict

Make a filtering decision after seeing all of the outbound data for a flow.

### Handling remediation

func handleRemediation(for: NEFilterFlow) -> NEFilterRemediationVerdict

Handle a remediation request.

### Handling rule updates

func handleRulesChanged()

Handle a rules changed event.

### Changing filter settings

func apply(NEFilterSettings?, completionHandler: ((any Error)?) -> Void)

Applies a set of filtering rules associated with the provider and changes the default filtering action.

class NEFilterSettings

The rules and other settings that define the operation of a filter.

### Resuming data flows

func resumeFlow(NEFilterFlow, with: NEFilterVerdict)

Resumes a previously-paused flow.

### Updating filter verdicts

func update(NEFilterSocketFlow, using: NEFilterDataVerdict, for: NETrafficDirection)

Updates the verdict for a flow outside the context of any filter data provider callback.

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

class NEFilterControlProvider

The principal class for a filter control provider extension.

class NEFilterPacketProvider

A filter provider that evaluates network packets and decides whether to block, allow, or delay the packets.

class NEFilterProvider

An abstract base class shared by content filters.

