

- System Configuration
-  SCPreferencesNotification 

Structure

# SCPreferencesNotification

The type of notification (used with the SCPreferencesCallBack callback).

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct SCPreferencesNotification
```

## Mentioned in 

notificationType

## Topics

### Constants

static var commit: SCPreferencesNotification

Indicates when new preferences have been saved.

static var apply: SCPreferencesNotification

Indicates when a request has been made to apply the currently saved preferences to the active system configuration.

### Initializers

init(rawValue: UInt32)

Creates a preferences notification structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

