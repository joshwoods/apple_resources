

- Foundation
- NSLocale
-  object(forKey:) 

Instance Method

# object(forKey:)

Returns the value of the component corresponding to the specified key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func object(forKey key: NSLocale.Key) -> Any?
```

## Parameters 

`key`  

The component for which to return the corresponding value. For possible values, see NSLocale.Key.

## Return Value

The object corresponding to `key`.

## See Also

### Accessing Locale Information by Key

func displayName(forKey: NSLocale.Key, value: Any) -> String?

Returns the display name for the given locale component value.

struct Key

The keys used to access components of a locale.

