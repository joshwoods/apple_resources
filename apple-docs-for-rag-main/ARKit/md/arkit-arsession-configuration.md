

- ARKit
- ARSession
-  configuration 

Instance Property

# configuration

An object that defines motion and scene tracking behaviors for the session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@NSCopying
var configuration: ARConfiguration? { get }
```

## See Also

### Configuring and running a session

func run(ARConfiguration, options: ARSession.RunOptions)

Starts AR processing for the session with the specified configuration and options.

var identifier: UUID

A unique identifier of the running session.

struct RunOptions

Options for transitioning an AR session’s current state when you change its configuration.

func pause()

Pauses processing in the session.

