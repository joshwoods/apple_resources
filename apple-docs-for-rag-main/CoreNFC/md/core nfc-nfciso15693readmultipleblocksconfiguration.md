

- Core NFC
-  NFCISO15693ReadMultipleBlocksConfiguration 

Class

# NFCISO15693ReadMultipleBlocksConfiguration

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
class NFCISO15693ReadMultipleBlocksConfiguration
```

## Overview

Configuration options for the Read Multiple Blocks command.

## Topics

### Initializers

init(range: NSRange, chunkSize: Int)

init(range: NSRange, chunkSize: Int, maximumRetries: Int, retryInterval: TimeInterval)

### Instance Properties

var chunkSize: Int

var range: NSRange

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

