

- Foundation
- Bundle
-  loadNibNamed(\_:owner:topLevelObjects:) 

Instance Method

# loadNibNamed(\_:owner:topLevelObjects:)

Loads a nib from the bundle with the specified file name and owner.

macOS 10.8+

``` source
func loadNibNamed(
    _ nibName: NSNib.Name,
    owner: Any?,
    topLevelObjects: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

## Parameters 

`nibName`  

The name of the nib.

`owner`  

The object that will be the nib’s owner.

`topLevelObjects`  

This by-reference parameter is populated with the top level objects of the nib.

## Return Value

true if the nib file was loaded successfully; otherwise, false.

## Discussion

Unlike legacy methods, the objects adhere to the standard cocoa memory management rules; it is necessary to keep a strong reference to them by using IBOutlets or holding a reference to the array to prevent the nib contents from being deallocated.

Outlets to top-level objects should be strong references to demonstrate ownership and prevent deallocation.

For more information on Nibs, see NSNib.

## See Also

### Loading Nib Files

func loadNibNamed(String, owner: Any?, options: [UINib.OptionsKey : Any]?) -> [Any]?

Unarchives the contents of a nib file located in the receiver’s bundle.

