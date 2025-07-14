

- SwiftUI
-  UIHostingConfiguration 

Structure

# UIHostingConfiguration

A content configuration suitable for hosting a hierarchy of SwiftUI views.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
struct UIHostingConfiguration where Content : View, Background : View
```

## Overview

Use a value of this type, which conforms to the UIContentConfiguration protocol, with a UICollectionViewCell or UITableViewCell to host a hierarchy of SwiftUI views in a collection or table view, respectively. For example, the following shows a stack with an image and text inside the cell:

```
myCell.contentConfiguration = UIHostingConfiguration {
    HStack {
        Image(systemName: "star").foregroundStyle(.purple)
        Text("Favorites")
        Spacer()
    }
}
```

You can also customize the background of the containing cell. The following example draws a blue background:

```
myCell.contentConfiguration = UIHostingConfiguration {
    HStack {
        Image(systemName: "star").foregroundStyle(.purple)
        Text("Favorites")
        Spacer()
    }
}
.background {
    Color.blue
}
```

When used in a list layout, certain APIs are bridged automatically, like swipe actions and separator alignment. The following example shows a trailing yellow star swipe action:

```
cell.contentConfiguration = UIHostingConfiguration {
    HStack {
        Image(systemName: "airplane")
        Text("Flight 123")
        Spacer()
    }
    .swipeActions {
        Button { ... } label: {
            Label("Favorite", systemImage: "star")
        }
        .tint(.yellow)
    }
}
```

## Topics

### Creating and updating a configuration

init(content: () -> Content)

Creates a hosting configuration with the given contents.

### Setting the background

func background&lt;S>(S) -> UIHostingConfiguration&lt;Content, _UIHostingConfigurationBackgroundView&lt;S>>

Sets the background contents for the hosting configuration’s enclosing cell.

func background&lt;B>(content: () -> B) -> UIHostingConfiguration&lt;Content, B>

Sets the background contents for the hosting configuration’s enclosing cell.

### Setting margins

func margins(_:_:)

Sets the margins around the content of the configuration.

### Setting a size

func minSize(width: CGFloat?, height: CGFloat?) -> UIHostingConfiguration&lt;Content, Background>

Sets the minimum size for the configuration.

func minSize() -> UIHostingConfiguration&lt;Content, Background>

Sets the minimum size for the configuration.

Deprecated

## Relationships

### Conforms To

- UIContentConfiguration

## See Also

### Displaying SwiftUI views in UIKit

Using SwiftUI with UIKit

Learn how to incorporate SwiftUI views into a UIKit app.

Unifying your app’s animations

Create a consistent UI animation experience across SwiftUI, UIKit, and AppKit.

class UIHostingController

A UIKit view controller that manages a SwiftUI view hierarchy.

struct UIHostingControllerSizingOptions

Options for how a hosting controller tracks its content’s size.

