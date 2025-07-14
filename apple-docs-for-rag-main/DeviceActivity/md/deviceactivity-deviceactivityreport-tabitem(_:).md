

- DeviceActivity
- DeviceActivityReport
-  tabItem(\_:) 

Instance Method

# tabItem(\_:)

Sets the tab bar item associated with this view.

DeviceActivitySwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+watchOS 7.0–11.4Deprecated

``` source
nonisolated
func tabItem(@ViewBuilder _ label: () -> V) -> some View where V : View
```

## Parameters 

`label`  

The tab bar item to associate with this view.

## Discussion

Use `tabItem(_:)` to configure a view as a tab bar item in a `TabView`. The example below adds two views as tabs in a `TabView`:

```
struct View1: View {
    var body: some View {
        Text("View 1")
    }
}

struct View2: View {
    var body: some View {
        Text("View 2")
    }
}

struct TabItem: View {
    var body: some View {
        TabView {
            View1()
                .tabItem {
                    Label("Menu", systemImage: "list.dash")
                }

            View2()
                .tabItem {
                    Label("Order", systemImage: "square.and.pencil")
                }
        }
    }
}
```

