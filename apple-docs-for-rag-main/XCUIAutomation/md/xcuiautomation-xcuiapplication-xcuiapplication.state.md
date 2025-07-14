

- XCUIAutomation
- XCUIApplication
-  XCUIApplication.State 

Enumeration

# XCUIApplication.State

The possible states of an application during UI testing.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
enum State
```

## Topics

### Enumeration cases

case unknown

The application’s current state is unknown.

case notRunning

The application isn’t running.

case runningBackgroundSuspended

The application is running in the background, but is suspended.

case runningBackground

The application is running in the background.

case runningForeground

The application is running in the foreground.

### Initializers

init?(rawValue: UInt)

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

### Determining application state

var state: XCUIApplication.State

The most recent state of the application.

