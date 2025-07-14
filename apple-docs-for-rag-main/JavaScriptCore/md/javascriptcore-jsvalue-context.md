

- JavaScriptCore
- JSValue
-  context 

Instance Property

# context

The JavaScript context hosting this value.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var context: JSContext! { get }
```

## Discussion

A value maintains a strong reference to its enclosing JavaScript environment (a JSContext object). As such, you should not store JavaScript values inside objects that are owned by the same JSContext object, as this action creates a retain cycle. To properly manage memory when storing JSValue instances, use the JSManagedValue class.

You can pass a value to other JavaScript contexts with the same virtual machine, but not to contexts with other virtual machines. Use the virtualMachine property of a value’s context to determine which other contexts can use the value.

