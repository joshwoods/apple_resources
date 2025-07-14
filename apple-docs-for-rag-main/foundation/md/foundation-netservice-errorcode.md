

- Foundation
- NetService
-  errorCode 

Type Property

# errorCode

This key identifies the error that occurred during the most recent operation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
class let errorCode: String
```

## See Also

### Constants

class let errorDomain: String

This key identifies the originator of the error, which is either the `NSNetService` object or the mach network layer. For most errors, you should not need the value provided by this key.

