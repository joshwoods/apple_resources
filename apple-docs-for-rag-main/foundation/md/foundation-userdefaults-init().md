

- Foundation
- UserDefaults
-  init() 

Initializer

# init()

Creates a user defaults object initialized with the defaults for the app and current user.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init()
```

## Discussion

This initializer is equivalent to passing `nil` to the init(suiteName:) initializer.

Use this initializer only if you’re not using the shared standard user defaults.

## See Also

### Related Documentation

class var standard: UserDefaults

Returns the shared defaults object.

### Creating User Defaults Objects

init?(suiteName: String?)

Creates a user defaults object initialized with the defaults for the specified database name.

