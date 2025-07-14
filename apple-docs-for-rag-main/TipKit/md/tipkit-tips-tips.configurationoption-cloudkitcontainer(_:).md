

- TipKit
- Tips
- Tips.ConfigurationOption
-  cloudKitContainer(\_:) 

Type Method

# cloudKitContainer(\_:)

Sets the CloudKit container used for syncing tips.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func cloudKitContainer(_ cloudKitContainer: Tips.ConfigurationOption.CloudKitContainer?) -> Tips.ConfigurationOption
```

## Parameters 

`cloudKitContainer`  

The option to use for specifying TipKit’s CloudKit datastore. Use `nil` to disable CloudKit syncing.

## Overview

Use `cloudKitContainer` to sync TipKit’s datastore across devices.

In order to avoid record collisions between your app and TipKit, it is recommended that you use a separate container for syncing tips.

By default, TipKit’s datastore does not sync with CloudKit.

## Discussion

Syncing TipKit’s datastore requires two separate capabilities in your app’s entitlements: the iCloud capability which lets you specify a CloudKit container, and the Background Modes capability, which lets your app receive remote notifications from CloudKit that contain information about new changes on the server.

```
@main
struct TipKitTrails: App {
    init() {
        do {
            // Sync the TipKit datastore using CloudKit.
            try Tips.configure([
                .cloudKitContainer(.named("iCloud.com.apple.TipKitTrails.tips"))
            ])
        }
        catch {
            // Handle TipKit errors
            print("Error initializing TipKit \(error.localizedDescription)")
        }
    }
}
```

### CloudKit Container Values

## See Also

### Configuration

static func configure([Tips.ConfigurationOption]) throws

Loads and configures the persistent state of all tips in your app.

static func datastoreLocation(Tips.ConfigurationOption.DatastoreLocation) -> Tips.ConfigurationOption

Specify a custom location for your tips datastore.

static func displayFrequency(Tips.ConfigurationOption.DisplayFrequency) -> Tips.ConfigurationOption

Customizes how often new tips are presented in your app after another tip has been displayed.

