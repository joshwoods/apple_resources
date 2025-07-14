

- AppKit
- NSPrintInfo
-  dictionary() 

Instance Method

# dictionary()

Returns the print info’s dictionary that contains the printing attributes.

macOS

``` source
func dictionary() -> NSMutableDictionary
```

## Discussion

The key-value pairs contained in the dictionary are described in Constants. Modifying the returned dictionary changes the receiver’s attributes.

This dictionary is key-value observing compliant.

