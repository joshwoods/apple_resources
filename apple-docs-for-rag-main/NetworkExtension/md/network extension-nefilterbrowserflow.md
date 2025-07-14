

- Network Extension
-  NEFilterBrowserFlow 

Class

# NEFilterBrowserFlow

A flow of network data, originating from a WebKit-based browser, that the filter examines.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class NEFilterBrowserFlow
```

## Topics

### Getting browser flow properties

var parentURL: URL?

A URL of the web page that’s responsible for the flow’s creation.

var request: URLRequest?

An HTTP request of the flow.

var response: URLResponse?

An HTTP response of the flow.

## Relationships

### Inherits From

- NEFilterFlow

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Flow handling

class NEFilterFlow

The abstract base class for types that represent flows of network data.

class NEFilterSocketFlow

A flow of network data that the filter examines.

class NEFilterNewFlowVerdict

The result from a filter data provder after the initial examination of a flow.

class NEFilterDataVerdict

The result from a filter data provder for subsequent chunks of data on a flow.

class NEFilterControlVerdict

The result from a filter control provider.

class NEFilterRemediationVerdict

The result from a filter data provider after the user requests remediation for a blocked flow.

class NEFilterVerdict

The abstract base class for filter verdict classes.

class NEFilterReport

The report of the data provider’s action on a flow.

