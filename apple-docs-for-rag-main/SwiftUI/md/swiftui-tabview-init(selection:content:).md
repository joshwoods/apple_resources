

- SwiftUI
- TabView
-  init(selection:content:) 

Initializer

# init(selection:content:)

Creates a tab view that uses a builder to create and specify selection values for its tabs.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    selection: Binding,
    @TabContentBuilder content: () -> C
) where Content == TabContentBuilder.Content, C : TabContent
```

Show all declarations

## Parameters 

`selection`  

The selection in the TabView. The value of this binding must match the `value` of the tabs in `content`.

`content`  

The Tab content.

## See Also

### Creating a tab view

init(content:)

Creates a tab view that uses a builder to create its tabs.

