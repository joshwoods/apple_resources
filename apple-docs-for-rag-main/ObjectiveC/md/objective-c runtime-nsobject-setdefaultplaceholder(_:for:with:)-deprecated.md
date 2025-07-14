

- Objective-C Runtime
- NSObject
-  setDefaultPlaceholder(\_:for:with:) Deprecated

Type Method

# setDefaultPlaceholder(\_:for:with:)

Sets `placeholder` as the default placeholder for the `binding`, when a key value coding compliant property of an instance of the receiving class returns the value specified by `marker`, and no other placeholder has been specified.

macOS 10.0–11.0Deprecated

``` source
class func setDefaultPlaceholder(
    _ placeholder: Any?,
    for marker: Any?,
    with binding: NSBindingName
)
```

## Discussion

The `marker` can be `nil` or one of the constants described in Selection Markers.

## See Also

### Related Documentation

Cocoa Bindings Programming Topics

### Deprecated Class Methods

class func defaultPlaceholder(for: Any?, with: NSBindingName) -> Any?

Returns an object that will be used as the placeholder for the `binding`, when a key value coding compliant property of an instance of the receiving class returns the value specified by `marker`, and no other placeholder has been specified.

Deprecated

class func useStoredAccessor() -> Bool

Returns `true` if the stored value methods storedValue(forKey:) and takeStoredValue(_:forKey:) should use private accessor methods in preference to public accessors.

Deprecated

