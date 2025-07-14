

- SwiftUI
- DynamicViewContent
-  onInsert(of:perform:) Deprecated

Instance Method

# onInsert(of:perform:)

Sets the insert action for the dynamic view.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
func onInsert(
    of acceptedTypeIdentifiers: [String],
    perform action: @escaping (Int, [NSItemProvider]) -> Void
) -> some DynamicViewContent
```

Deprecated

Use onInsert(of:perform:) instead.

Show all declarations

## Parameters 

`acceptedTypeIdentifiers`  

An array of UTI types that the dynamic view supports.

`action`  

A closure that SwiftUI invokes when elements are added to the view. The closure takes two arguments: The first argument is the offset relative to the dynamic view’s underlying collection of data. The second argument is an array of `NSItemProvider` that represents the data that you want to insert.

## Return Value

A view that calls `action` when elements are inserted into the original view.

