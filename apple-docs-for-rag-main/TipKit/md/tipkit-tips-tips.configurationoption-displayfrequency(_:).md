

- TipKit
- Tips
- Tips.ConfigurationOption
-  displayFrequency(\_:) 

Type Method

# displayFrequency(\_:)

Customizes how often new tips are presented in your app after another tip has been displayed.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func displayFrequency(_ displayFrequency: Tips.ConfigurationOption.DisplayFrequency) -> Tips.ConfigurationOption
```

## Overview

Use `displayFrequency` to control how often new tips are displayed. For example, if display frequency is set to `.daily` and your `FavoriteLandmarkTip` is displayed, no new tips will be shown for at least 24 hours.

Display frequency only applies to tips that have not appeared. Previously displayed tips will still appear if their display rules are satisfied.

Individual tips can override this behavior by specifying Tips.IgnoresDisplayFrequency in their options.

The default value for this option is immediate.

Display frequency can be set using configure(_:):

```
@main
struct SampleApp: App {
    init() {
        do {
            // Configure your tips with a daily display frequency.
            try Tips.configure([
                .displayFrequency(.daily)
            ])
        }
        catch {
            // Handle TipKit errors
            print("Error initializing TipKit \(error.localizedDescription)")
        }
    }
}
```

### Display Frequency Values

static var immediate: Tips.ConfigurationOption.DisplayFrequency

An immediate display frequency.

static var daily: Tips.ConfigurationOption.DisplayFrequency

A daily display frequency.

static var hourly: Tips.ConfigurationOption.DisplayFrequency

A hourly display frequency.

static var weekly: Tips.ConfigurationOption.DisplayFrequency

A weekly display frequency.

static var monthly: Tips.ConfigurationOption.DisplayFrequency

A monthly display frequency.

## See Also

### Configuration

static func configure([Tips.ConfigurationOption]) throws

Loads and configures the persistent state of all tips in your app.

static func cloudKitContainer(Tips.ConfigurationOption.CloudKitContainer?) -> Tips.ConfigurationOption

Sets the CloudKit container used for syncing tips.

static func datastoreLocation(Tips.ConfigurationOption.DatastoreLocation) -> Tips.ConfigurationOption

Specify a custom location for your tips datastore.

