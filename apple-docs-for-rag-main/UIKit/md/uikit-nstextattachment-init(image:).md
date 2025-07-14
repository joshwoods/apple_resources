

- UIKit
- NSTextAttachment
-  init(image:) 

Initializer

# init(image:)

Creates a text attachment object to contain the specified image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
init(image: UIImage)
```

## Parameters 

`image`  

The image for the attachment.

## Return Value

A new text attachment object initialized with the image.

## Discussion

Attachments created with this method automatically adapt to the surrounding font and color attributes in attributed strings.

For example, the following code creates a text attachment from the UIImage class using an SF symbol in a blue headline style and embeds it at the end of the NSMutableAttributedString class:

```
let content = NSMutableAttributedString(string: "Open ")
guard let lockImage = UIImage(systemName: "lock") else {
    return
}
let attributes: [NSAttributedString.Key: Any] = [
    .foregroundColor: UIColor.blue,
    .font: UIFont.preferredFont(forTextStyle: .headline)
]
let lockSymbol = NSMutableAttributedString(
    attachment: NSTextAttachment(image: lockImage)
)
lockSymbol.addAttributes(attributes, 
                         range: NSRange(location: 0, length: 1))
content.insert(lockSymbol, at: 5)

```

## See Also

### Initializing a text attachment

convenience init(fileWrapper: FileWrapper?)

Creates a text attachment object to contain the specified file wrapper.

init(data: Data?, ofType: String?)

Creates a text attachment object with the specified data.

