

- SwiftUI
- GroupBox
-  init(label:content:) Deprecated

Initializer

# init(label:content:)

iOS 14.0–18.4DeprecatediPadOS 14.0–18.4DeprecatedMac Catalyst 14.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
nonisolated
init(
    label: Label,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` conforms to `View` and `Content` conforms to `View`.

