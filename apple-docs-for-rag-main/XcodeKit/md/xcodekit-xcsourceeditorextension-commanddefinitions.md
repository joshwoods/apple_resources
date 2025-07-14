

- XcodeKit
- XCSourceEditorExtension
-  commandDefinitions 

Instance Property

# commandDefinitions

The array of command definitions used by Xcode to associate command names with their implementation in an extension.

macOS 10.12+

``` source
optional var commandDefinitions: [[XCSourceEditorCommandDefinitionKey : Any]] { get }
```

## Discussion

Implement this property when you need to override the command definitions specified in your extension target’s Info.plist file. There are no guarantees about the thread or queue on which this property is accessed.

## See Also

### Related Documentation

struct XCSourceEditorCommandDefinitionKey

A key in the dictionary that defines a source editor command.

