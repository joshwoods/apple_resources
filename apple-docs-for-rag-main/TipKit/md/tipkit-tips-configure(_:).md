

- TipKit
- Tips
-  configure(\_:) 

Type Method

# configure(\_:)

Loads and configures the persistent state of all tips in your app.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func configure(_ configuration: [Tips.ConfigurationOption] = []) throws
```

## Parameters 

`configuration`  

An array of options for customizing your tip’s datastore location and default frequency control interval.

## Discussion

Note

This function must be called before tips display in your app.

Call this function during app initialization. By default, all tips persist to a default location with a display frequency of immediate.

```
@main
struct SampleApp: App {
    init() {
        do {
            // Configure tips in the app.
            try Tips.configure()
        }
        catch {
            // Handle TipKit errors
            print("Error initializing TipKit \(error.localizedDescription)")
        }
    }
}
```

To change the default location of where your tips persist use the convenience method datastoreLocation(_:).

To change the display frequency use the convenience method displayFrequency(_:).

```
do {
    // Configure tips in the app.
    try Tips.configure([
        .datastoreLocation(.groupContainer(identifier: "MyGroupContainer")),
        .displayFrequency(.hourly)
    ])
}
catch {
    // Handle TipKit errors
    print("Error initializing TipKit \(error.localizedDescription)")
}
```

## See Also

### Configuration

static func cloudKitContainer(Tips.ConfigurationOption.CloudKitContainer?) -> Tips.ConfigurationOption

Sets the CloudKit container used for syncing tips.

static func datastoreLocation(Tips.ConfigurationOption.DatastoreLocation) -> Tips.ConfigurationOption

Specify a custom location for your tips datastore.

static func displayFrequency(Tips.ConfigurationOption.DisplayFrequency) -> Tips.ConfigurationOption

Customizes how often new tips are presented in your app after another tip has been displayed.

