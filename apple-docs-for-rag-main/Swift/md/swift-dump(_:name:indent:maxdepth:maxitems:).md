

- Swift
-  dump(\_:name:indent:maxDepth:maxItems:) 

Function

# dump(\_:name:indent:maxDepth:maxItems:)

Dumps the given object’s contents using its mirror to standard output.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
func dump(
    _ value: T,
    name: String? = nil,
    indent: Int = 0,
    maxDepth: Int = .max,
    maxItems: Int = .max
) -> T
```

## Parameters 

`value`  

The value to output to the `target` stream.

`name`  

A label to use when writing the contents of `value`. When `nil` is passed, the label is omitted. The default is `nil`.

`indent`  

The number of spaces to use as an indent for each line of the output. The default is `0`.

`maxDepth`  

The maximum depth to descend when writing the contents of a value that has nested components. The default is `Int.max`.

`maxItems`  

The maximum number of elements for which to write the full contents. The default is `Int.max`.

## Return Value

The instance passed as `value`.

## See Also

### Printing and Dumping

func print(Any..., separator: String, terminator: String)

Writes the textual representations of the given items into the standard output.

func print&lt;Target>(Any..., separator: String, terminator: String, to: inout Target)

Writes the textual representations of the given items into the given output stream.

func debugPrint(Any..., separator: String, terminator: String)

Writes the textual representations of the given items most suitable for debugging into the standard output.

func debugPrint&lt;Target>(Any..., separator: String, terminator: String, to: inout Target)

Writes the textual representations of the given items most suitable for debugging into the given output stream.

func dump&lt;T, TargetStream>(T, to: inout TargetStream, name: String?, indent: Int, maxDepth: Int, maxItems: Int) -> T

Dumps the given object’s contents using its mirror to the specified output stream.

