

- SwiftUI
- View
-  navigationTitle(\_:) 

Instance Method

# navigationTitle(\_:)

Configures the view’s title for purposes of navigation, using a string binding.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func navigationTitle(_ title: Binding) -> some View
```

Show all declarations

## Parameters 

`title`  

The text of the title.

## Discussion

In iOS, iPadOS, and macOS, this allows editing the navigation title when the title is displayed in the toolbar.

Refer to the Configure your apps navigation titles article for more information on navigation title modifiers.

## See Also

### Setting titles for navigation content

func navigationSubtitle(_:)

Configures the view’s subtitle for purposes of navigation.

func navigationDocument(_:)

Configures the view’s document for purposes of navigation.

func navigationDocument(_:preview:)

Configures the view’s document for purposes of navigation.

