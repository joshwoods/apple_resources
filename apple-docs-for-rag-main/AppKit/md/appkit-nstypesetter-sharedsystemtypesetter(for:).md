

- AppKit
- NSTypesetter
-  sharedSystemTypesetter(for:) 

Type Method

# sharedSystemTypesetter(for:)

Returns a shared instance of a reentrant typesetter that implements typesetting with the specified behavior.

macOS

``` source
class func sharedSystemTypesetter(for behavior: NSLayoutManager.TypesetterBehavior) -> Any
```

## Parameters 

`behavior`  

The desired behavior.

## Return Value

A shared instance of a reentrant typesetter that implements typesetting with the specified behavior.

## Discussion

Possible return values are described in the NSLayoutManager.TypesetterBehavior section for NSLayoutManager.

## See Also

### Related Documentation

var typesetterBehavior: NSLayoutManager.TypesetterBehavior

Returns the current typesetter behavior.

### Getting a typesetter

class var sharedSystemTypesetter: NSTypesetter

Returns a shared instance of a reentrant typesetter.

