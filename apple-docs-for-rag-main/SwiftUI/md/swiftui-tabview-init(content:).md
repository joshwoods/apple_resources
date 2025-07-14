

- SwiftUI
- TabView
-  init(content:) 

Initializer

# init(content:)

Creates a tab view that uses a builder to create its tabs.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(@TabContentBuilder content: () -> C) where SelectionValue == Never, Content == TabContentBuilder.Content, C : TabContent
```

Available when `SelectionValue` conforms to `Hashable` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`content`  

The Tab content.

## See Also

### Creating a tab view

init(selection:content:)

Creates a tab view that uses a builder to create and specify selection values for its tabs.

