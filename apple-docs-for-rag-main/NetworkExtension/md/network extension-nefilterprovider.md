

- Network Extension
-  NEFilterProvider 

Class

# NEFilterProvider

An abstract base class shared by content filters.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class NEFilterProvider
```

## Overview

A Network Content Filter is made up of two Filter Provider extensions:

The **Filter Data Provider extension** examines network content as it passes through the network stack on the device and decides if the network content should be blocked or allowed to pass on to its final destination.

Because the Filter Data Provider extension has access to all of the network content flowing through the device, it runs in a very restrictive sandbox. The sandbox prevents the Filter Data Provider extension from moving network content outside of its address space by blocking all network access, IPC, and disk write operations.

The Filter Data Provider extension is implemented by creating a custom subclass of the NEFilterDataProvider class.

The **Filter Control Provider extension** is responsible for feeding information to the Filter Data Provider extension so that the Filter Data Provider extension can do its job.

For example, the Filter Control Provider extension can be notified by the Filter Data Provider extension that it does not have enough information to make a decision about a particular flow of network content. The Filter Control Provider extension can then download more filtering rules from a server and write the rules to a location where the Filter Data Provider can access them.

The Filter Control Provider extension is implemented by creating a custom subclass of the NEFilterControlProvider class.

Important

To use the NEFilterProvider class, you must enable the Network Extensions capability in Xcode and select the Content Filter capability. See Configure network extensions.

### Subclassing Notes

`NEFilterProvider` should not be subclassed directly. Instead, you should create subclasses of `NEFilterProvider’s` subclasses and override the following methods:

#### Methods to Override

- startFilter(completionHandler:)

- stopFilter(with:completionHandler:)

## Topics

### Managing the filter life cycle

func startFilter(completionHandler: ((any Error)?) -> Void)

Start the filter.

func stopFilter(with: NEProviderStopReason, completionHandler: () -> Void)

Stop the filter.

### Getting the filter configuration

var filterConfiguration: NEFilterProviderConfiguration

An NEFilterProviderConfiguration object containing the current filter configuration.

### Receiving reports

func handle(NEFilterReport)

Receives a report from the framework.

### Handling errors

let NEFilterErrorDomain: String

The domain for errors resulting from calls to the filter manager.

enum NEFilterManagerError

Error codes specific to filter managers.

## Relationships

### Inherits From

- NEProvider

### Inherited By

- NEFilterControlProvider
- NEFilterDataProvider
- NEFilterPacketProvider

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

class NEFilterControlProvider

The principal class for a filter control provider extension.

class NEFilterPacketProvider

A filter provider that evaluates network packets and decides whether to block, allow, or delay the packets.

