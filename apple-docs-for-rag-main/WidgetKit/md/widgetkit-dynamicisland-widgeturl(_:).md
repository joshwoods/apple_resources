

- WidgetKit
- DynamicIsland
-  widgetURL(\_:) 

Instance Method

# widgetURL(\_:)

Sets the URL that opens the corresponding app of a Live Activity when a user taps on the Live Activity.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
func widgetURL(_ url: URL?) -> DynamicIsland
```

## Parameters 

`url`  

The URL that opens the app.

## Return Value

The configuration object for the Dynamic Island with the specified URL.

## Discussion

By setting the URL with this function, it becomes the default URL for deep linking into the app for each view of the Live Activity. However, if you include a Link in the Live Activity, the link takes priority over the default URL. When a person taps on the `Link`, it takes them to the place in the app that corresponds to the URL of the `Link`.

