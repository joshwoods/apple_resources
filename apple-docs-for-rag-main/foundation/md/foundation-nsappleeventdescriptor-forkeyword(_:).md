

- Foundation
- NSAppleEventDescriptor
-  forKeyword(\_:) 

Instance Method

# forKeyword(\_:)

Returns the receiver’s descriptor for the specified keyword.

Mac Catalyst 13.0+macOS 10.0+

``` source
func forKeyword(_ keyword: AEKeyword) -> NSAppleEventDescriptor?
```

## Parameters 

`keyword`  

A keyword (a four-character code) that identifies the descriptor to obtain.

## Return Value

A descriptor for the specified keyword, or `nil` if an error occurs.

## See Also

### Working With Record Descriptors

func keywordForDescriptor(at: Int) -> AEKeyword

Returns the keyword for the descriptor at the specified (one-based) position in the receiver.

func remove(withKeyword: AEKeyword)

Removes the receiver’s descriptor identified by the specified keyword.

func setDescriptor(NSAppleEventDescriptor, forKeyword: AEKeyword)

Adds a descriptor, identified by a keyword, to the receiver.

