

- ARKit
- ARSession
-  ARSession.RunOptions 

Structure

# ARSession.RunOptions

Options for transitioning an AR session’s current state when you change its configuration.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
struct RunOptions
```

## Topics

### Creating Run Options

init(rawValue: UInt)

Creates a run options.

### Run Options

static var resetTracking: ARSession.RunOptions

An option to reset the device’s position from the session’s previous run.

static var removeExistingAnchors: ARSession.RunOptions

An option to remove any anchor objects associated with the session’s previous run.

static var stopTrackedRaycasts: ARSession.RunOptions

An option to stop all active tracked raycasts.

static var resetSceneReconstruction: ARSession.RunOptions

An option to reset the scene mesh.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Configuring and running a session

func run(ARConfiguration, options: ARSession.RunOptions)

Starts AR processing for the session with the specified configuration and options.

var identifier: UUID

A unique identifier of the running session.

var configuration: ARConfiguration?

An object that defines motion and scene tracking behaviors for the session.

func pause()

Pauses processing in the session.

