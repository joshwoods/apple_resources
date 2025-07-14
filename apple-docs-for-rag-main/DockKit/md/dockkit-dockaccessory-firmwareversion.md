

- DockKit
- DockAccessory
-  firmwareVersion 

Instance Property

# firmwareVersion

The firmware version of the dock accessory.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
final var firmwareVersion: String? { get }
```

## Discussion

The format of the version is major, minor, and revision, separated by periods.

## See Also

### Getting accessory information

var hardwareModel: String?

The model of the dock accessory.

let identifier: DockAccessory.Identifier

The name and unique identifer of the dock accessory.

struct Identifier

Information that uniquely identifies the dock accessory.

enum Category

Types of supported dock accesories.

enum State

The state of a dock accessory.

struct StateChange

An event that indicates a change in the state of a dock accessory.

struct StateChanges

An asynchronous sequence of dock accessory state changes.

