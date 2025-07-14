

- Foundation
- NSPositionalSpecifier
-  insertionReplaces 

Instance Property

# insertionReplaces

Returns a Boolean value that indicates whether evaluation has been successful and the object to be inserted should actually replace the keyed, indexed object in the insertion container.

Mac Catalyst 13.0+macOS 10.0+

``` source
var insertionReplaces: Bool { get }
```

## Return Value

true if evaluation has been successful and the object to be inserted should actually replace the keyed, indexed object in the insertion container, instead of being inserted before it; false otherwise.

## Discussion

If this object has never been evaluated, evaluation is attempted.

## See Also

### Accessing information about a positional specifier

var insertionContainer: Any?

Returns the container in which the new or copied object or objects should be placed.

var insertionIndex: Int

Returns an insertion index that indicates where the new or copied object or objects should be placed.

var insertionKey: String?

Returns the key that identifies the relationship into which the new or copied object or objects should be inserted.

var objectSpecifier: NSScriptObjectSpecifier

Returns the object specifier specified at initialization time.

var position: NSPositionalSpecifier.InsertionPosition

Returns the insertion position specified at initialization time.

func setInsertionClassDescription(NSScriptClassDescription)

Sets the class description for the object or objects to be inserted.

