

- Foundation
- NSPositionalSpecifier
-  insertionIndex 

Instance Property

# insertionIndex

Returns an insertion index that indicates where the new or copied object or objects should be placed.

Mac Catalyst 13.0+macOS 10.0+

``` source
var insertionIndex: Int { get }
```

## Return Value

An insertion index. Determined by evaluating the receiver.

## See Also

### Accessing information about a positional specifier

var insertionContainer: Any?

Returns the container in which the new or copied object or objects should be placed.

var insertionKey: String?

Returns the key that identifies the relationship into which the new or copied object or objects should be inserted.

var insertionReplaces: Bool

Returns a Boolean value that indicates whether evaluation has been successful and the object to be inserted should actually replace the keyed, indexed object in the insertion container.

var objectSpecifier: NSScriptObjectSpecifier

Returns the object specifier specified at initialization time.

var position: NSPositionalSpecifier.InsertionPosition

Returns the insertion position specified at initialization time.

func setInsertionClassDescription(NSScriptClassDescription)

Sets the class description for the object or objects to be inserted.

