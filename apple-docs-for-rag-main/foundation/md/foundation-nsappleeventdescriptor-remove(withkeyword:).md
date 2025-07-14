

- Foundation
- NSAppleEventDescriptor
-  remove(withKeyword:) 

Instance Method

# remove(withKeyword:)

Removes the receiver’s descriptor identified by the specified keyword.

Mac Catalyst 13.0+macOS 10.0+

``` source
func remove(withKeyword keyword: AEKeyword)
```

## Parameters 

`keyword`  

A keyword (a four-character code) that identifies the descriptor to remove.

## Discussion

The receiver must be an Apple event or Apple event record. Currently provides no indication if an error occurs.

## See Also

### Working With Record Descriptors

func forKeyword(AEKeyword) -> NSAppleEventDescriptor?

Returns the receiver’s descriptor for the specified keyword.

func keywordForDescriptor(at: Int) -> AEKeyword

Returns the keyword for the descriptor at the specified (one-based) position in the receiver.

func setDescriptor(NSAppleEventDescriptor, forKeyword: AEKeyword)

Adds a descriptor, identified by a keyword, to the receiver.

