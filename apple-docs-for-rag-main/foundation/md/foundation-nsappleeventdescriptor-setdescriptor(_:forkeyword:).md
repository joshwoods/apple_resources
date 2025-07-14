

- Foundation
- NSAppleEventDescriptor
-  setDescriptor(\_:forKeyword:) 

Instance Method

# setDescriptor(\_:forKeyword:)

Adds a descriptor, identified by a keyword, to the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func setDescriptor(
    _ descriptor: NSAppleEventDescriptor,
    forKeyword keyword: AEKeyword
)
```

## Parameters 

`descriptor`  

The descriptor to add to the receiver.

`keyword`  

A keyword (a four-character code) that identifies the descriptor to add. If a descriptor with that keyword already exists in the receiver, it is replaced.

## Discussion

The receiver must be an Apple event or Apple event record. Currently provides no indication if an error occurs.

## See Also

### Working With Record Descriptors

func forKeyword(AEKeyword) -> NSAppleEventDescriptor?

Returns the receiver’s descriptor for the specified keyword.

func keywordForDescriptor(at: Int) -> AEKeyword

Returns the keyword for the descriptor at the specified (one-based) position in the receiver.

func remove(withKeyword: AEKeyword)

Removes the receiver’s descriptor identified by the specified keyword.

