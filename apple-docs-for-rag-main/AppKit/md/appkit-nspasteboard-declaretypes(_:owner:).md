

- AppKit
- NSPasteboard
-  declareTypes(\_:owner:) 

Instance Method

# declareTypes(\_:owner:)

Prepares the receiver for a change in its contents by declaring the new types of data it will contain and a new owner.

macOS

``` source
func declareTypes(
    _ newTypes: [NSPasteboard.PasteboardType],
    owner newOwner: Any?
) -> Int
```

## Parameters 

`newTypes`  

An array of `NSString` objects that specify the types of data that may be added to the new pasteboard. The types should be ordered according to the preference of the source application, with the most preferred type coming first (typically, the richest representation).

`newOwner`  

The object responsible for writing data to the pasteboard, or `nil` if you provide data for all types immediately. If you specify a `newOwner` object, it must support all of the types declared in the `newTypes` parameter and must remain alive for as long as the data is *promised* on the pasteboard.

## Return Value

The receiver’s new change count.

## Discussion

This method is the equivalent of invoking clearContents(), implicitly writing the first pasteboard item, and then calling addTypes(_:owner:) to promise types for the first pasteboard item.

Note

In macOS 10.5 and earlier, this method is the first step in writing data to the pasteboard and must precede the messages that actually write the data. A declareTypes(_:owner:) message essentially changes the contents of the receiver: It invalidates the current contents of the receiver and increments its change count.

### Special Considerations

In general, you should not use this method with writeObjects(_:), since writeObjects(_:) will always write additional items to the pasteboard, and will not affect items already on the pasteboard, including the item implicitly created by this method.

## See Also

### Related Documentation

func clearContents() -> Int

Clears the existing contents of the pasteboard.

var changeCount: Int

The receiver’s change count.

### Writing Data (macOS 10.5 and Earlier)

func addTypes([NSPasteboard.PasteboardType], owner: Any?) -> Int

Adds promises for the specified types to the first pasteboard item.

func writeFileContents(String) -> Bool

Writes the contents of the specified file to the pasteboard.

func write(FileWrapper) -> Bool

Writes the serialized contents of the specified file wrapper to the pasteboard.

