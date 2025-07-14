

- Foundation
- Formatter
-  editingString(for:) 

Instance Method

# editingString(for:)

The default implementation of this method invokes string(for:).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func editingString(for obj: Any) -> String?
```

## Parameters 

`obj`  

The object for which to return an editing string.

## Return Value

An `NSString` object that is used for editing the textual representation of `anObject`.

## Discussion

When implementing a subclass, override this method only when the string that users see and the string that they edit are different. In your implementation, return an `NSString` object that is used for editing, following the logic recommended for implementing string(for:). As an example, you would implement this method if you want the dollar signs in displayed strings removed for editing.

## See Also

### Getting Textual Representations of Object Values

func string(for: Any?) -> String?

The default implementation of this method raises an exception.

func attributedString(for: Any, withDefaultAttributes: [NSAttributedString.Key : Any]?) -> NSAttributedString?

The default implementation returns `nil` to indicate that the formatter object does not provide an attributed string.

