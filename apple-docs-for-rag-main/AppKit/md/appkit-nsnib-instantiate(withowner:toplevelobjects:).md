

- AppKit
- NSNib
-  instantiate(withOwner:topLevelObjects:) 

Instance Method

# instantiate(withOwner:topLevelObjects:)

Instantiates objects in the nib file with the specified owner.

macOS 10.8+

``` source
func instantiate(
    withOwner owner: Any?,
    topLevelObjects: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

## Parameters 

`owner`  

The object to set as the Nib’s owner (File’s Owner).

`topLevelObjects`  

On return, an array containing the top-level objects of the nib.

## Return Value

true if the nib is instantiated; otherwise false.

## Discussion

Unlike legacy methods, the objects adhere to standard Cocoa memory management rules; it is necessary to keep a strong reference to the objects or the array to prevent the nib contents from being deallocated.

Outlets to top level objects should be strong references to demonstrate ownership and prevent deallocation.

