

- Social
- SLComposeServiceViewController
-  textView 

Instance Property

# textView

The editable text view in the compose view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+

**iOS, iPadOS, Mac Catalyst**

``` source
@MainActor
var textView: UITextView! { get }
```

**macOS**

``` source
@MainActor
var textView: NSTextView! { get }
```

## Discussion

When a user activates a Post or Send button, you can send their text by sending `self.textView.text`. Note that the `SLComposeServiceViewController` base class creates `textView` in its loadView() method and sets itself to be the `textView` delegate.

## See Also

### Managing the Contents of the Post

var contentText: String!

A string that represents the text which the user entered into the compose view’s text view.

var placeholder: String!

A string that’s displayed in the compose view’s text view when the text view is empty.

