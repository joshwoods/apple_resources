

- Swift
-  print(\_:separator:terminator:to:) 

Function

# print(\_:separator:terminator:to:)

Writes the textual representations of the given items into the given output stream.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func print(
    _ items: Any...,
    separator: String = " ",
    terminator: String = "\n",
    to output: inout Target
) where Target : TextOutputStream
```

## Parameters 

`items`  

Zero or more items to print.

`separator`  

A string to print between each item. The default is a single space (`" "`).

`terminator`  

The string to print after all items have been printed. The default is a newline (`"\n"`).

`output`  

An output stream to receive the text representation of each item.

## Discussion

You can pass zero or more items to the `print(_:separator:terminator:to:)` function. The textual representation for each item is the same as that obtained by calling `String(describing: item)`. The following example prints a closed range of integers to a string:

```
var range = "My range: "
print(1...5, to: &range)
// range == "My range: 1...5\n"
```

To print the items separated by something other than a space, pass a string as `separator`.

```
var separated = ""
print(1.0, 2.0, 3.0, 4.0, 5.0, separator: " ... ", to: &separated)
// separated == "1.0 ... 2.0 ... 3.0 ... 4.0 ... 5.0\n"
```

The output from each call to `print(_:separator:terminator:to:)` includes a newline by default. To print the items without a trailing newline, pass an empty string as `terminator`.

```
var numbers = ""
for n in 1...5 {
    print(n, terminator: "", to: &numbers)
}
// numbers == "12345"
```

## See Also

### Printing and Dumping

func print(Any..., separator: String, terminator: String)

Writes the textual representations of the given items into the standard output.

func debugPrint(Any..., separator: String, terminator: String)

Writes the textual representations of the given items most suitable for debugging into the standard output.

func debugPrint&lt;Target>(Any..., separator: String, terminator: String, to: inout Target)

Writes the textual representations of the given items most suitable for debugging into the given output stream.

func dump&lt;T>(T, name: String?, indent: Int, maxDepth: Int, maxItems: Int) -> T

Dumps the given object’s contents using its mirror to standard output.

func dump&lt;T, TargetStream>(T, to: inout TargetStream, name: String?, indent: Int, maxDepth: Int, maxItems: Int) -> T

Dumps the given object’s contents using its mirror to the specified output stream.

