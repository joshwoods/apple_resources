

- AppKit
- NSText
-  paste(\_:) 

Instance Method

# paste(\_:)

This action method pastes text from the general pasteboard at the insertion point or over the selection.

macOS

``` source
@MainActor
func paste(_ sender: Any?)
```

## See Also

### Action methods for editing

func selectAll(Any?)

This action method selects all of the receiver’s text.

func copy(Any?)

This action method copies the selected text onto the general pasteboard, in as many formats as the receiver supports.

func cut(Any?)

This action method deletes the selected text and places it onto the general pasteboard, in as many formats as the receiver supports.

func copyFont(Any?)

This action method copies the font information for the first character of the selection (or for the insertion point) onto the font pasteboard, as `NSFontPboardType`.

func pasteFont(Any?)

This action method pastes font information from the font pasteboard onto the selected text or insertion point of a rich text object, or over all text of a plain text object.

func copyRuler(Any?)

This action method copies the paragraph style information for first selected paragraph onto the ruler pasteboard, as `NSRulerPboardType`, and expands the selection to paragraph boundaries.

func pasteRuler(Any?)

This action method pastes paragraph style information from the ruler pasteboard onto the selected paragraphs of a rich text object.

func delete(Any?)

This action method deletes the selected text.

