

- UIKit
- UIApplication
-  UIApplication.State 

Enumeration

# UIApplication.State

Constants that indicate the running states of an app.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
enum State
```

## Topics

### Constants

case active

The app is running in the foreground and currently receiving events.

case inactive

The app is running in the foreground but isn’t receiving events.

case background

The app is running in the background.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the application state

var applicationState: UIApplication.State

The app’s current state, or that of its most active scene.

