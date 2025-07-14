

- Core NFC
-  NFCISO15693CustomCommandConfiguration 

Class

# NFCISO15693CustomCommandConfiguration

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class NFCISO15693CustomCommandConfiguration
```

## Overview

Configuration options for the Manufacturer Custom command.

## Topics

### Initializers

init(manufacturerCode: Int, customCommandCode: Int, requestParameters: Data?)

init(manufacturerCode: Int, customCommandCode: Int, requestParameters: Data?, maximumRetries: Int, retryInterval: TimeInterval)

### Instance Properties

var customCommandCode: Int

var manufacturerCode: Int

var requestParameters: Data

## Relationships

### Inherits From

- NFCTagCommandConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

