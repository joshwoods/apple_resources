

- Foundation
- ValueTransformer
-  init(forName:) 

Initializer

# init(forName:)

Returns the value transformer identified by a given identifier.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(forName name: NSValueTransformerName)
```

## Parameters 

`name`  

The transformer identifier.

## Return Value

The value transformer identified by `name` in the shared registry, or `nil` if not found.

## Discussion

If `valueTransformerForName:` does not find a registered transformer instance for `name`, it will attempt to find a class with the specified name. If a corresponding class is found an instance will be created and initialized using its `init:` method and then automatically registered with `name`.

## See Also

### Using the Name-Based Registry

class func setValueTransformer(ValueTransformer?, forName: NSValueTransformerName)

Registers the provided value transformer with a given identifier.

class func valueTransformerNames() -> [NSValueTransformerName]

Returns an array of all the registered value transformers.

struct NSValueTransformerName

Named value transformers defined by `NSValueTransformer`.

