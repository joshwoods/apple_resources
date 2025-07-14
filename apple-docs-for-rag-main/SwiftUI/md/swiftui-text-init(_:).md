

- SwiftUI
- Text
-  init(\_:) 

Initializer

# init(\_:)

Creates a text view that displays styled attributed content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(_ attributedContent: AttributedString)
```

Show all declarations

## Parameters 

`attributedContent`  

An attributed string to style and display, in accordance with its attributes.

## Discussion

Use this initializer to style text according to attributes found in the specified AttributedString. Attributes in the attributed string take precedence over styles added by view modifiers. For example, the attributed text in the following example appears in blue, despite the use of the foregroundColor(_:) modifier to use red throughout the enclosing VStack:

```
var content: AttributedString {
    var attributedString = AttributedString("Blue text")
    attributedString.foregroundColor = .blue
    return attributedString
}

var body: some View {
    VStack {
        Text(content)
        Text("Red text")
    }
    .foregroundColor(.red)
}
```

SwiftUI combines text attributes with SwiftUI modifiers whenever possible. For example, the following listing creates text that is both bold and red:

```
var content: AttributedString {
    var content = AttributedString("Some text")
    content.inlinePresentationIntent = .stronglyEmphasized
    return content
}

var body: some View {
    Text(content).foregroundColor(Color.red)
}
```

A SwiftUI Text view renders most of the styles defined by the Foundation attribute inlinePresentationIntent, like the stronglyEmphasized value, which SwiftUI presents as bold text.

Important

Text uses only a subset of the attributes defined in AttributeScopes.FoundationAttributes. `Text` renders all InlinePresentationIntent attributes except for lineBreak and softBreak. It also renders the link attribute as a clickable link. `Text` ignores any other Foundation-defined attributes in an attributed string.

SwiftUI also defines additional attributes in the attribute scope AttributeScopes.SwiftUIAttributes which you can access from an attributed string’s swiftUI property. SwiftUI attributes take precedence over equivalent attributes from other frameworks, such as AttributeScopes.UIKitAttributes and AttributeScopes.AppKitAttributes.

You can create an `AttributedString` with Markdown syntax, which allows you to style distinct runs within a `Text` view:

```
let content = try! AttributedString(
    markdown: "**Thank You!** Please visit our [website](http://example.com).")

var body: some View {
    Text(content)
}
```

The `**` syntax around “Thank You!” applies an inlinePresentationIntent attribute with the value stronglyEmphasized. SwiftUI renders this as bold text, as described earlier. The link syntax around “website” creates a link attribute, which `Text` styles to indicate it’s a link; by default, clicking or tapping the link opens the linked URL in the user’s default browser. Alternatively, you can perform custom link handling by putting an OpenURLAction in the text view’s environment.

You can also use Markdown syntax in localized string keys, which means you can write the above example without needing to explicitly create an `AttributedString`:

```
var body: some View {
    Text("**Thank You!** Please visit our [website](https://example.com).")
}
```

In your app’s strings files, use Markdown syntax to apply styling to the app’s localized strings. You also use this approach when you want to perform automatic grammar agreement on localized strings, with the `^[text](inflect:true)` syntax.

For details about Markdown syntax support in SwiftUI, see init(_:tableName:bundle:comment:).

## See Also

### Creating a text view

init(LocalizedStringKey, tableName: String?, bundle: Bundle?, comment: StaticString?)

Creates a text view that displays localized content identified by a key.

init(verbatim: String)

Creates a text view that displays a string literal without localization.

init(Date, style: Text.DateStyle)

Creates an instance that displays localized dates and times using a specific style.

init(_:format:)

Creates a text view that displays the formatted representation of a nonstring type supported by a corresponding format style.

init(_:formatter:)

Creates a text view that displays the formatted representation of a Foundation object.

init(timerInterval: ClosedRange&lt;Date>, pauseTime: Date?, countsDown: Bool, showsHours: Bool)

Creates an instance that displays a timer counting within the provided interval.

