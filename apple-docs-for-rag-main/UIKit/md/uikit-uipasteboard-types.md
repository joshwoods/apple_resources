

- UIKit
- UIPasteboard
-  types 

Instance Property

# types

The types of the first item on the pasteboard.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var types: [String] { get }
```

## Return Value

An array of strings indicating the representation types of the first item on the pasteboard.

## Discussion

A type is frequently, but not necessarily, a UTI (Uniform Type Identifier). It identifies a representation of the data on the pasteboard. For example, a pasteboard item could hold image data under `public.png` and `public.tiff` representations. Apps can define their own types for custom data such as `com.mycompany.myapp.mytype`; however, in this case, only those apps that know of the type could understand the data written to the pasteboard.

With this method, you can determine if the pasteboard holds data of a particular representation type by a line of code such as this:

```
BOOL pngOnPasteboard = [[pasteboard pasteboardTypes] containsObject:@"public.png"];
```

Starting in iOS 10, you can directly check which data types are present on a pasteboard by using the convenience methods described in Checking for data types on a pasteboard.

## See Also

### Determining types of pasteboard items

func types(forItemSet: IndexSet?) -> [[String]]?

Returns an array of representation types for each specified pasteboard item.

func contains(pasteboardTypes: [String]) -> Bool

Returns whether the pasteboard holds data of the specified representation type.

func contains(pasteboardTypes: [String], inItemSet: IndexSet?) -> Bool

Returns whether the specified pasteboard items contain data of the given representation types.

func itemSet(withPasteboardTypes: [String]) -> IndexSet?

Returns an index set identifying pasteboard items having the specified representation types.

