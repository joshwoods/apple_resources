

- BrowserEngineKit
- BETextInput
-  insertTextPlaceholder(size:completionHandler:) 

Instance Method

# insertTextPlaceholder(size:completionHandler:)

Inserts a placeholder object to reserve visual space during text input. If `size.height` is less than or equal to zero, then the placeholder is inline and line height. If `size.height` is greather than zero, then the placeholder is treated as a paragraph of height `size.height`.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func insertTextPlaceholder(
    size: CGSize,
    completionHandler: @escaping (UITextPlaceholder) -> Void
)
```

``` source
func insertTextPlaceholder(size: CGSize) async -> UITextPlaceholder
```

**Required**

## See Also

### Text placeholders

func remove(UITextPlaceholder, willInsertText: Bool, completionHandler: () -> Void)

Removes a placeholder object from the text input view.

**Required**

