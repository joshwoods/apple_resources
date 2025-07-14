

- Core NFC
- CardSession
-  isSupported 

Type Property

# isSupported

A property that indicates whether the current device supports card session functionality.

iOS 17.4+iPadOS 17.4+

``` source
class var isSupported: Bool { get }
```

## Discussion

Query this property before calling init() to avoid raising fatalError(_:file:line:) on ineligible devices.

## See Also

### Determining card session availability

static var isEligible: Bool

A property that indicates whether the current system supports card session functionality.

