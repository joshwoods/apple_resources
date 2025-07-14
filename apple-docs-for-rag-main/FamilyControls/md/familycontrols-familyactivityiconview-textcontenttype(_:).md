

- FamilyControls
- FamilyActivityIconView
-  textContentType(\_:) 

Instance Method

# textContentType(\_:)

Sets the text content type for this view, which the system uses to offer suggestions while the user enters text on an iOS or tvOS device.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+

``` source
nonisolated
func textContentType(_ textContentType: UITextContentType?) -> some View
```

## Parameters 

`textContentType`  

One of the content types available in the UITextContentType structure that identify the semantic meaning expected for a text-entry area. These include support for email addresses, location names, URLs, and telephone numbers, to name just a few.

## Discussion

Use this method to set the content type for input text. For example, you can configure a `TextField` for the entry of email addresses:

```
TextField("Enter your email", text: $emailAddress)
    .textContentType(.emailAddress)
```

