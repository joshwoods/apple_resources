

- Automator
- AMShellScriptAction
-  remapLineEndings 

Instance Property

# remapLineEndings

A Boolean value that indicates whether you want automatic remapping of carriage return (`\r`) to newline (`\n`) characters in the input string.

Mac Catalyst 14.0+macOS 10.4+

``` source
var remapLineEndings: Bool { get }
```

## Discussion

The default is false. Override to return true if you want the remapping to occur.

## See Also

### Handling the I/O Separator Character

var inputFieldSeparator: String

A string to use as the delimiter between items in the string passed to the action through standard input.

var outputFieldSeparator: String

A string to use as a delimiter in the string output by the action.

