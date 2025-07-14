

- GameKit
-  GKReleaseState 

Structure

# GKReleaseState

Describes the release state of an App Store Connect resource, such as an Achievement or Leaderboard.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
struct GKReleaseState
```

## Topics

### Initializers

init(rawValue: UInt)

### Type Properties

static var prereleased: GKReleaseState

The resource has been created in App Store Connect but isn’t yet associated with a released version of an App.

static var released: GKReleaseState

The resource is associated with a release in App Store Connect. This has no relationship with the “archived” state of a resource (i.e., A resource can be release *and* archived).

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

