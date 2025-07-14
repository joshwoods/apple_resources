

- Foundation
- NSAppleEventDescriptor
-  keywordForDescriptor(at:) 

Instance Method

# keywordForDescriptor(at:)

Returns the keyword for the descriptor at the specified (one-based) position in the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func keywordForDescriptor(at index: Int) -> AEKeyword
```

## Parameters 

`index`  

The one-based descriptor list position of the descriptor to get the keyword for.

## Return Value

The keyword (a four-character code) for the descriptor at the one-based location specified by `anIndex`, or 0 if an error occurs.

## See Also

### Working With Record Descriptors

func forKeyword(AEKeyword) -> NSAppleEventDescriptor?

Returns the receiver’s descriptor for the specified keyword.

func remove(withKeyword: AEKeyword)

Removes the receiver’s descriptor identified by the specified keyword.

func setDescriptor(NSAppleEventDescriptor, forKeyword: AEKeyword)

Adds a descriptor, identified by a keyword, to the receiver.

