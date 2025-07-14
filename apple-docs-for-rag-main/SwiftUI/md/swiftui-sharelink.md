

- SwiftUI
-  ShareLink 

Structure

# ShareLink

A view that controls a sharing presentation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
struct ShareLink where Data : RandomAccessCollection, PreviewImage : Transferable, PreviewIcon : Transferable, Label : View, Data.Element : Transferable
```

## Overview

People tap or click on a share link to present a share interface. The link typically uses a system-standard appearance; you only need to supply the content to share:

```
ShareLink(item: URL(string: "https://developer.apple.com/xcode/swiftui/")!)
```

You can control the appearance of the link by providing view content. For example, you can use a Label to display a link with a custom icon:

```
ShareLink(item: URL(string: "https://developer.apple.com/xcode/swiftui/")!) {
    Label("Share", image: "MyCustomShareIcon")
}
```

If you only wish to customize the link’s title, you can use one of the convenience initializers that takes a string and creates a `Label` for you:

```
ShareLink("Share URL", item: URL(string: "https://developer.apple.com/xcode/swiftui/")!)
```

The link can share any content that is Transferable. Many framework types, like URL, already conform to this protocol. You can also make your own types transferable.

For example, you can use ProxyRepresentation to resolve your own type to a framework type:

```
struct Photo: Transferable {
    static var transferRepresentation: some TransferRepresentation {
        ProxyRepresentation(\.image)
    }

    public var image: Image
    public var caption: String
}

struct PhotoView: View {
    let photo: Photo

    var body: View {
        photo.image
            .toolbar {
                ShareLink(
                    item: photo,
                    preview: SharePreview(
                        photo.caption,
                        image: photo.image))
            }
    }
}
```

Sometimes the content that your app shares isn’t immediately available. You can use FileRepresentation or DataRepresentation when you need an asynchronous operation, like a network request, to retrieve and prepare the content.

A `Transferable` type also lets you provide multiple content types for a single shareable item. The share interface shows relevant sharing services based on the types that you provide.

The previous example also shows how you provide a preview of your content to show in the share interface.

A preview isn’t required when sharing URLs or non-attributed strings. When sharing these types of content, the system can automatically determine a preview.

You can provide a preview even when it’s optional. For instance, when sharing URLs, the automatic preview first shows a placeholder link icon alongside the base URL while fetching the link’s metadata over the network. The preview updates once the link’s icon and title become available. If you provide a preview instead, the preview appears immediately without fetching data over the network.

Some share activities support subject and message fields. You can pre-populate these fields with the `subject` and `message` parameters:

```
ShareLink(
    item: photo,
    subject: Text("Cool Photo"),
    message: Text("Check it out!")
    preview: SharePreview(
        photo.caption,
        image: photo.image))
```

## Topics

### Sharing an item

init(item:subject:message:)

Creates an instance that presents the share interface.

init(_:item:subject:message:)

Creates an instance, with a custom label, that presents the share interface.

init(item:subject:message:label:)

Creates an instance that presents the share interface.

### Sharing an item with a preview

init&lt;I>(item: I, subject: Text?, message: Text?, preview: SharePreview&lt;PreviewImage, PreviewIcon>)

Creates an instance that presents the share interface.

init(_:item:subject:message:preview:)

Creates an instance, with a custom label, that presents the share interface.

init&lt;I>(item: I, subject: Text?, message: Text?, preview: SharePreview&lt;PreviewImage, PreviewIcon>, label: () -> Label)

Creates an instance that presents the share interface.

### Sharing items

init(items:subject:message:)

Creates an instance that presents the share interface.

init(_:items:subject:message:)

Creates an instance, with a custom label, that presents the share interface.

init(items:subject:message:label:)

Creates an instance that presents the share interface.

### Sharing items with a preview

init(items: Data, subject: Text?, message: Text?, preview: (Data.Element) -> SharePreview&lt;PreviewImage, PreviewIcon>)

Creates an instance that presents the share interface.

init(_:items:subject:message:preview:)

Creates an instance, with a custom label, that presents the share interface.

init(items: Data, subject: Text?, message: Text?, preview: (Data.Element) -> SharePreview&lt;PreviewImage, PreviewIcon>, label: () -> Label)

Creates an instance that presents the share interface.

### Supporting types

struct DefaultShareLinkLabel

The default label used for a share link.

## Relationships

### Conforms To

- View

## See Also

### Linking to other content

struct Link

A control for navigating to a URL.

struct SharePreview

A representation of a type to display in a share preview.

struct TextFieldLink

A control that requests text input from the user when pressed.

struct HelpLink

A button with a standard appearance that opens app-specific help documentation.

