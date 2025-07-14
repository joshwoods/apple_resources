

- SwiftUI
- View
-  navigationSubtitle(\_:) 

Instance Method

# navigationSubtitle(\_:)

Configures the view’s subtitle for purposes of navigation.

Mac Catalyst 14.0+macOS 11.0+

``` source
nonisolated
func navigationSubtitle(_ subtitle: Text) -> some View
```

Show all declarations

## Parameters 

`subtitle`  

The subtitle to display.

## Discussion

A view’s navigation subtitle is used to provide additional contextual information alongside the navigation title. On macOS, the primary destination’s subtitle is displayed with the navigation title in the titlebar.

## See Also

### Setting titles for navigation content

func navigationTitle(_:)

Configures the view’s title for purposes of navigation, using a string binding.

func navigationDocument(_:)

Configures the view’s document for purposes of navigation.

func navigationDocument(_:preview:)

Configures the view’s document for purposes of navigation.

