

- AppKit
- NSUserDefaultsController
-  init(defaults:initialValues:) 

Initializer

# init(defaults:initialValues:)

Returns an initialized NSUserDefaultsController object using the NSUserDefaults instance specified in `defaults` and the initial default values contained in the `initialValues` dictionary.

macOS

``` source
init(
    defaults: UserDefaults?,
    initialValues: [String : Any]?
)
```

## Discussion

If `defaults` is `nil`, the receiver uses `[NSUserDefaults standardUserDefaults]`.

This method is the designated initializer.

## See Also

### Initializing a user defaults controller

init?(coder: NSCoder)

