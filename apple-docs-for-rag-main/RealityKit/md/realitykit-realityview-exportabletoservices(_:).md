

- RealityKit
- RealityView
-  exportableToServices(\_:) 

Instance Method

# exportableToServices(\_:)

Exports items for consumption by shortcuts, quick actions, and services.

RealityKitSwiftUImacOS 13.0+

``` source
nonisolated
func exportableToServices(_ payload: @autoclosure @escaping () -> [T]) -> some View where T : Transferable
```

## Parameters 

`payload`  

A closure that will be called on request of the items by the shortcut or service.

## Discussion

If the associated view supports selection, the exported item should reflect that selected subpart.

```
var title: String
var body: some View {
    Color.pink
        .frame(width: 400, height: 400)
        .exportableToServices([title])
}
```

