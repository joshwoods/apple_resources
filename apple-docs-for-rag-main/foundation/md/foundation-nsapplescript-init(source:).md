

- Foundation
- NSAppleScript
-  init(source:) 

Initializer

# init(source:)

Initializes a newly allocated script instance from the passed source.

Mac Catalyst 13.0+macOS 10.0+

``` source
init?(source: String)
```

## Parameters 

`source`  

A string containing the source code of a script.

## Return Value

The initialized script object, `nil` if an error occurs.

## Discussion

This method is a designated initializer for `NSAppleScript`.

## See Also

### Initializing a Script

init?(contentsOf: URL, error: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?)

Initializes a newly allocated script instance from the source identified by the passed URL.

