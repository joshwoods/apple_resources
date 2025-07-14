

- BrowserEngineKit
- BETextInput
-  remove(\_:willInsertText:completionHandler:) 

Instance Method

# remove(\_:willInsertText:completionHandler:)

Removes a placeholder object from the text input view.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func remove(
    _ placeholder: UITextPlaceholder,
    willInsertText: Bool,
    completionHandler: @escaping () -> Void
)
```

``` source
func remove(
    _ placeholder: UITextPlaceholder,
    willInsertText: Bool
) async
```

**Required**

## See Also

### Text placeholders

func insertTextPlaceholder(size: CGSize, completionHandler: (UITextPlaceholder) -> Void)

Inserts a placeholder object to reserve visual space during text input. If `size.height` is less than or equal to zero, then the placeholder is inline and line height. If `size.height` is greather than zero, then the placeholder is treated as a paragraph of height `size.height`.

**Required**

