

- AppKit
- NSApplicationDelegate
-  application(\_:delegateHandlesKey:) 

Instance Method

# application(\_:delegateHandlesKey:)

Returns a Boolean value that indicates if the app supports the specified scripting key.

macOS

``` source
@MainActor
optional func application(
    _ sender: NSApplication,
    delegateHandlesKey key: String
) -> Bool
```

## Parameters 

`sender`  

The app object associated with the delegate.

`key`  

The key to be handled.

## Return Value

true if your delegate handles the key or false if it does not.

## Discussion

Implement this method and return true if your delegate handles the specified `key`, Your delegate must be able get or set the scriptable property or element that corresponds to that key. You need to handle only your app’s custom commands. The app already implements methods for each of the keys that it handles, where the method name matches the key.

For example, a scriptable app that doesn’t use Cocoa’s document-based app architecture can implement this method to supply its own document ordering. You want to do this because the standard app delegate expects to work with a document-based app. The TextEdit app (whose source is distributed with macOS developer tools) provides the following implementation:

```
return [key isEqualToString:@"orderedDocuments"];
```

TextEdit then implements the `orderedDocuments` method in its controller class to return an ordered list of documents. An app with its own window ordering might add a test for the key `orderedWindows` so that its delegate can provide its own version of `orderedWindows`.

Important

Cocoa scripting does not invoke this method for script commands other than `get` or `set`. For information on working with other commands, see Script Commands in Cocoa Scripting Guide.

