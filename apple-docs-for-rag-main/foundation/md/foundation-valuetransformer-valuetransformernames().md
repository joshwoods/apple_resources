

- Foundation
- ValueTransformer
-  valueTransformerNames() 

Type Method

# valueTransformerNames()

Returns an array of all the registered value transformers.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func valueTransformerNames() -> [NSValueTransformerName]
```

## Return Value

An array of all the registered value transformers.

## See Also

### Using the Name-Based Registry

class func setValueTransformer(ValueTransformer?, forName: NSValueTransformerName)

Registers the provided value transformer with a given identifier.

init?(forName: NSValueTransformerName)

Returns the value transformer identified by a given identifier.

struct NSValueTransformerName

Named value transformers defined by `NSValueTransformer`.

