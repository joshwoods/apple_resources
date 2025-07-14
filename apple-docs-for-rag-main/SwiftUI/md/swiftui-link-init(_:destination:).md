

- SwiftUI
- Link
-  init(\_:destination:) 

Initializer

# init(\_:destination:)

Creates a control, consisting of a URL and a title key, used to navigate to a URL.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    destination: URL
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the localized title that describes the purpose of this link.

`destination`  

The URL for the link.

## Discussion

Use Link to create a control that your app uses to navigate to a URL that you provide. The example below creates a link to `example.com` and uses `Visit Example Co` as the title key to generate a link-styled view in your app:

```
Link("Visit Example Co",
      destination: URL(string: "https://www.example.com/")!)
```

## See Also

### Creating a link

init(destination: URL, label: () -> Label)

Creates a control, consisting of a URL and a label, used to navigate to the given URL.

