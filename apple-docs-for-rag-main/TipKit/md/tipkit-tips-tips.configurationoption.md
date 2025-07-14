

- TipKit
- Tips
-  Tips.ConfigurationOption 

Structure

# Tips.ConfigurationOption

A type that marks an object as a tip configuration.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ConfigurationOption
```

## Topics

### Structures

struct CloudKitContainer

A type for specifying the CloudKit container used for syncing tips.

struct DatastoreLocation

A type for specifying a custom location for your tips datastore.

struct DisplayFrequency

A type for specifying the minimum duration after one tip is shown before another tip will become eligible.

### Type Methods

static func cloudKitContainer(Tips.ConfigurationOption.CloudKitContainer?) -> Tips.ConfigurationOption

Sets the CloudKit container used for syncing tips.

static func datastoreLocation(Tips.ConfigurationOption.DatastoreLocation) -> Tips.ConfigurationOption

Specify a custom location for your tips datastore.

static func displayFrequency(Tips.ConfigurationOption.DisplayFrequency) -> Tips.ConfigurationOption

Customizes how often new tips are presented in your app after another tip has been displayed.

## Relationships

### Conforms To

- Sendable

## See Also

### Options

struct IgnoresDisplayFrequency

Controls whether a tip obeys the preconfigured display frequency interval.

struct MaxDisplayCount

Specifies the maximum number of times a tip displays before the system automatically invalidates it.

struct ParameterOption

A type that represents the various customizations that you can make to a tip parameter.

