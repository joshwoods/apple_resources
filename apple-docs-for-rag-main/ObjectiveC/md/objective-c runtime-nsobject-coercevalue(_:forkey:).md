

- Objective-C Runtime
- NSObject
-  coerceValue(\_:forKey:) 

Instance Method

# coerceValue(\_:forKey:)

Uses type info from the class description and `NSScriptCoercionHandler` to attempt to convert `value` for `key` to the proper type, if necessary.

Mac CatalystmacOS

``` source
func coerceValue(
    _ value: Any?,
    forKey key: String
) -> Any?
```

## Discussion

The method `coerceValueFor:` is used if it exists.

