

- TipKit
- Tips
- Tips.ConfigurationOption
-  datastoreLocation(\_:) 

Type Method

# datastoreLocation(\_:)

Specify a custom location for your tips datastore.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func datastoreLocation(_ storeLocation: Tips.ConfigurationOption.DatastoreLocation) -> Tips.ConfigurationOption
```

## Overview

Use `datastoreLocation` to change the on-disk location of your tips persistent storage.

By default `URL.applicationSupportDirectory` is used on macOS, iOS, watchOS, and visionOS.

On tvOS, `URL.cachesDirectory` is used by default in conjunction with `UserDefaults` to manage tip statuses.

```
@main
struct SampleApp: App {
    init() {
        do {
            // Save the tips datastore in a group container.
            try Tips.configure([
                .datastoreLocation(.groupContainer(identifier: "group.com.apple.TipKitTrails"))
            ])
        }
        catch {
            // Handle TipKit errors
            print("Error initializing TipKit \(error.localizedDescription)")
        }
    }
}
```

### Datastore Location Values

static var applicationDefault: Tips.ConfigurationOption.DatastoreLocation

The default location for persisting tips, which is generally your application’s support directory.

static func groupContainer(identifier: String) throws -> Tips.ConfigurationOption.DatastoreLocation

DatastoreLocation for persisting tips in a group container.

static func url(URL) -> Tips.ConfigurationOption.DatastoreLocation

DatastoreLocation for persisting tips at a custom URL.

## See Also

### Configuration

static func configure([Tips.ConfigurationOption]) throws

Loads and configures the persistent state of all tips in your app.

static func cloudKitContainer(Tips.ConfigurationOption.CloudKitContainer?) -> Tips.ConfigurationOption

Sets the CloudKit container used for syncing tips.

static func displayFrequency(Tips.ConfigurationOption.DisplayFrequency) -> Tips.ConfigurationOption

Customizes how often new tips are presented in your app after another tip has been displayed.

