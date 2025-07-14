

- Foundation
- NSAppleScript
-  init(contentsOf:error:) 

Initializer

# init(contentsOf:error:)

Initializes a newly allocated script instance from the source identified by the passed URL.

Mac Catalyst 13.0+macOS 10.0+

``` source
init?(
    contentsOf url: URL,
    error errorInfo: AutoreleasingUnsafeMutablePointer?
)
```

## Parameters 

`url`  

A URL that locates a script, in either text or compiled form.

`errorInfo`  

On return, if an error occurs, a pointer to an error information dictionary.

## Return Value

The initialized script object, `nil` if an error occurs.

## Discussion

This method is a designated initializer for `NSAppleScript`.

## See Also

### Related Documentation

Cocoa Scripting Guide

### Initializing a Script

init?(source: String)

Initializes a newly allocated script instance from the passed source.

