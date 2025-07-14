

- JavaScriptCore
- JSManagedValue
-  value 

Instance Property

# value

The managed value’s underlying JavaScript value.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var value: JSValue! { get }
```

## Discussion

If the JavaScript garbage collector removes the underlying value, this property becomes `nil`.

