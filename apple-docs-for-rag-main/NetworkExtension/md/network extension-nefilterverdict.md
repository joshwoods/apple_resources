

- Network Extension
-  NEFilterVerdict 

Class

# NEFilterVerdict

The abstract base class for filter verdict classes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class NEFilterVerdict
```

## Overview

Filter providers use instances this class to inform the system about how to handle flows of network data.

## Topics

### Configuring report generation

var shouldReport: Bool

A Boolean value that indicates whether to send a report to the control provider when processing this verdict.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NEFilterDataVerdict
- NEFilterNewFlowVerdict
- NEFilterRemediationVerdict

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

class NEFilterBrowserFlow

A flow of network data, originating from a WebKit-based browser, that the filter examines.

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

class NEFilterReport

The report of the data provider’s action on a flow.

