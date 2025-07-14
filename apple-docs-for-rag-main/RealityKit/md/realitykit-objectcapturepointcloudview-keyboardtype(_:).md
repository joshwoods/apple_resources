

- RealityKit
- ObjectCapturePointCloudView
-  keyboardType(\_:) 

Instance Method

# keyboardType(\_:)

Sets the keyboard type for this view.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+tvOS 13.0+

``` source
nonisolated
func keyboardType(_ type: UIKeyboardType) -> some View
```

## Parameters 

`type`  

One of the keyboard types defined in the UIKeyboardType enumeration.

## Discussion

Use `keyboardType(_:)` to specify the keyboard type to use for text entry. A number of different keyboard types are available to meet specialized input needs, such as entering email addresses or phone numbers.

The example below presents a `TextField` to input an email address. Setting the text field’s keyboard type to `.emailAddress` ensures the user can only enter correctly formatted email addresses.

```
TextField("someone@example.com", text: $emailAddress)
    .keyboardType(.emailAddress)
```

There are several different kinds of specialized keyboard types available though the UIKeyboardType enumeration. To specify the default system keyboard type, use `.default`.

