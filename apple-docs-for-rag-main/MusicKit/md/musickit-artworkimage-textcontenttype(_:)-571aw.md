

- MusicKit
- ArtworkImage
-  textContentType(\_:) 

Instance Method

# textContentType(\_:)

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on macOS.

MusicKitSwiftUImacOS 11.0+

``` source
nonisolated
func textContentType(_ textContentType: NSTextContentType?) -> some View
```

## Parameters 

`textContentType`  

One of the content types available in the NSTextContentType structure that identify the semantic meaning expected for a text-entry area.

## Discussion

Use this method to set the content type for input text. For example, you can configure a `TextField` for the entry of a username:

```
TextField("Enter your username", text: $username)
    .textContentType(.username)
```

