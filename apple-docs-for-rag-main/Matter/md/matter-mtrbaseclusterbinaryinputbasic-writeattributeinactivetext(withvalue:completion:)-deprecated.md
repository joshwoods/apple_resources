

- Matter
- MTRBaseClusterBinaryInputBasic
-  writeAttributeInactiveText(withValue:completion:) Deprecated

Instance Method

# writeAttributeInactiveText(withValue:completion:)

iOS 16.4–18.2DeprecatediPadOS 16.4–18.2DeprecatedMac Catalyst 16.4–18.2DeprecatedmacOS 13.3–15.2DeprecatedtvOS 16.4–18.2DeprecatedvisionOS 1.0–2.2DeprecatedwatchOS 9.4–11.2Deprecated

``` source
func writeAttributeInactiveText(
    withValue value: String,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func writeAttributeInactiveText(withValue value: String) async throws
```

Deprecated

This attribute is deprecated

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func writeAttributeInactiveText(withValue value: String) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

