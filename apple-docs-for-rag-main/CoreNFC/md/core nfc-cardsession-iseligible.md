

- Core NFC
- CardSession
-  isEligible 

Type Property

# isEligible

A property that indicates whether the current system supports card session functionality.

iOS 17.4+iPadOS 17.4+

``` source
static var isEligible: Bool { get async }
```

## Discussion

Query this property before calling init() to avoid showing a system card session UI on ineligible devices.

## See Also

### Determining card session availability

class var isSupported: Bool

A property that indicates whether the current device supports card session functionality.

