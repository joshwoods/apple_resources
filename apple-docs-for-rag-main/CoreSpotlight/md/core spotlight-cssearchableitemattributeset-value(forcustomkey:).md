

- Core Spotlight
- CSSearchableItemAttributeSet
-  value(forCustomKey:) 

Instance Method

# value(forCustomKey:)

Returns the value associated with the specified custom attribute key.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func value(forCustomKey key: CSCustomAttributeKey) -> (any NSSecureCoding)?
```

## Parameters 

`key`  

The custom attribute key.

## Return Value

The value associated with the custom attribute key.

## See Also

### Working with custom attributes

func setValue((any NSSecureCoding)?, forCustomKey: CSCustomAttributeKey)

Sets the value for a custom attribute key.

