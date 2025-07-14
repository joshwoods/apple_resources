

- Foundation
- ValueTransformer
-  setValueTransformer(\_:forName:) 

Type Method

# setValueTransformer(\_:forName:)

Registers the provided value transformer with a given identifier.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func setValueTransformer(
    _ transformer: ValueTransformer?,
    forName name: NSValueTransformerName
)
```

## Parameters 

`transformer`  

The transformer to register.

`name`  

The name for `transformer`.

## See Also

### Related Documentation

Value Transformer Programming Guide

### Using the Name-Based Registry

init?(forName: NSValueTransformerName)

Returns the value transformer identified by a given identifier.

class func valueTransformerNames() -> [NSValueTransformerName]

Returns an array of all the registered value transformers.

struct NSValueTransformerName

Named value transformers defined by `NSValueTransformer`.

