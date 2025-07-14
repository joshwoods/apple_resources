

- BrowserKit
- BEAvailability
-  BEAvailability.Context 

Enumeration

# BEAvailability.Context

The category of app for which you determine eligibility.

iOS 18.4+iPadOS 18.4+

``` source
enum Context
```

## Topics

### App categories

case webBrowser

The app is a web browser.

### Initialization

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Testing eligibility to use alternative browser engines

class BEAvailability

A class that tests whether a device is eligible to run an alternative browser engine.

