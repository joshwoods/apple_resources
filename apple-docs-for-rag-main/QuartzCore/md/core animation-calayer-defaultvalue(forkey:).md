

- Core Animation
- CALayer
-  defaultValue(forKey:) 

Type Method

# defaultValue(forKey:)

Specifies the default value associated with the specified key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class func defaultValue(forKey key: String) -> Any?
```

## Parameters 

`key`  

The name of one of the receiver’s properties.

## Return Value

The default value for the named property. Returns `nil` if no default value has been set.

## Discussion

If you define custom properties for a layer but do not set a value, this method returns a suitable “zero” default value based on the expected value of the `key`. For example, if the value for `key` is a CGSize struct, the method returns a size struct containing (0.0,0.0) wrapped in an NSValue object. For a CGRect an empty rectangle is returned. For CGAffineTransform and CATransform3D, the appropriate identity matrix is returned.

### Special Considerations

If `key` is not a known for property of the class, the result of the method is undefined.

## See Also

### Key-Value Coding Extensions

func shouldArchiveValue(forKey: String) -> Bool

Returns a Boolean indicating whether the value of the specified key should be archived.

