

- WidgetKit
-  ControlInfo 

Structure

# ControlInfo

A structure that contains information about user-configured controls.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
struct ControlInfo
```

## Topics

### Instance Properties

let kind: String

The string specified during creation of the control’s configuration.

var pushInfo: ControlPushInfo?

Push information about a control, if present.

### Instance Methods

func configurationIntent&lt;Intent>(of: Intent.Type) -> Intent?

Gets the associated App Intent.

### Default Implementations

Identifiable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Identifiable

## See Also

### Control configuration

struct StaticControlConfiguration

The description of a control widget that has no user-configurable options.

struct AppIntentControlConfiguration

The description of a control widget that uses a custom intent to provide user-configurable options.

