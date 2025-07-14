

- SceneKit
- SCNPhysicsWorld
-  SCNPhysicsWorld.TestOption 

Structure

# SCNPhysicsWorld.TestOption

Keys in options dictionaries that affect how SceneKit searches for bodies in a collision, ray, or sweep test.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct TestOption
```

## Discussion

Pass a dictionary containing one or more of these keys (with values as described above) for the `options` parameter when calling one of these methods:

- contactTestBetween(_:_:options:)

- contactTest(with:options:)

- rayTestWithSegment(from:to:options:)

- convexSweepTest(with:from:to:options:)

## Topics

### Type Properties

static let backfaceCulling: SCNPhysicsWorld.TestOption

The key for choosing whether to ignore back-facing polygons in physics shapes when searching for contacts.

static let collisionBitMask: SCNPhysicsWorld.TestOption

The key for selecting which categories of physics bodies that SceneKit should test for contacts.

static let searchMode: SCNPhysicsWorld.TestOption

The key for selecting the number and order of contacts to be tested.

struct TestSearchMode

Options affecting how SceneKit searches for bodies in a collision, ray, or sweep test, used with the searchMode key.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

