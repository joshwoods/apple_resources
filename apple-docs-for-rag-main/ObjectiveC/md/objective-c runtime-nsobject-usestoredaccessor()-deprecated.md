

- Objective-C Runtime
- NSObject
-  useStoredAccessor() Deprecated

Type Method

# useStoredAccessor()

Returns `true` if the stored value methods storedValue(forKey:) and takeStoredValue(_:forKey:) should use private accessor methods in preference to public accessors.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
class func useStoredAccessor() -> Bool
```

Deprecated

This method has no direct replacement, although see accessInstanceVariablesDirectly.

## Discussion

Returning NO causes the stored value methods to use the same accessor method or instance variable search order as the corresponding basic key-value coding methods (value(forKey:) and takeValue(_:forKey:)). The default implementation returns YES.

Applications should use the `valueForKey:` and `setValue:forKey:` methods instead of `storedValueForKey:` and `takeStoredValue:forKey:`.

## See Also

### Deprecated Class Methods

class func defaultPlaceholder(for: Any?, with: NSBindingName) -> Any?

Returns an object that will be used as the placeholder for the `binding`, when a key value coding compliant property of an instance of the receiving class returns the value specified by `marker`, and no other placeholder has been specified.

Deprecated

class func setDefaultPlaceholder(Any?, for: Any?, with: NSBindingName)

Sets `placeholder` as the default placeholder for the `binding`, when a key value coding compliant property of an instance of the receiving class returns the value specified by `marker`, and no other placeholder has been specified.

Deprecated

