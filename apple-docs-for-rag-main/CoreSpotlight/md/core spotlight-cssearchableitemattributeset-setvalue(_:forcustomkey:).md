

- Core Spotlight
- CSSearchableItemAttributeSet
-  setValue(\_:forCustomKey:) 

Instance Method

# setValue(\_:forCustomKey:)

Sets the value for a custom attribute key.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func setValue(
    _ value: (any NSSecureCoding)?,
    forCustomKey key: CSCustomAttributeKey
)
```

## Parameters 

`value`  

The value of the custom attribute. Values must be common property list types, such as NSString, NSNumber, NSNull, NSData, or NSDate, or an array of property list types.

`key`  

The custom attribute key.

## See Also

### Working with custom attributes

func value(forCustomKey: CSCustomAttributeKey) -> (any NSSecureCoding)?

Returns the value associated with the specified custom attribute key.

