

- SwiftUI
- View
-  workoutPreview(\_:isPresented:) 

Instance Method

# workoutPreview(\_:isPresented:)

Presents a preview of the workout contents as a modal sheet

WorkoutKitSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
nonisolated
func workoutPreview(
    _ workout: WorkoutPlan,
    isPresented: Binding
) -> some View
```

## Parameters 

`workout`  

The `WorkoutContainer` the preview displays

`isPresented`  

A binding to a Boolean value that determines whether to present the preview

## Discussion

```
struct WorkoutPreviewer: View {
    let workout: WorkoutPlan
    @State var presented: Bool = false
    var body: some View {
        Button {
            isPresented = true
        } label: {
            WorkoutContainerView(workout)
        }
        .workoutPreview(workout, isPresented: $presented)
    }
}
```

## See Also

### Accessing health data

func healthDataAccessRequest(store: HKHealthStore, objectType: HKObjectType, predicate: NSPredicate?, trigger: some Equatable, completion: (Result&lt;Bool, any Error>) -> Void) -> some View

Asynchronously requests permission to read a data type that requires per-object authorization (such as vision prescriptions).

func healthDataAccessRequest(store: HKHealthStore, readTypes: Set&lt;HKObjectType>, trigger: some Equatable, completion: (Result&lt;Bool, any Error>) -> Void) -> some View

Requests permission to read the specified HealthKit data types.

func healthDataAccessRequest(store: HKHealthStore, shareTypes: Set&lt;HKSampleType>, readTypes: Set&lt;HKObjectType>?, trigger: some Equatable, completion: (Result&lt;Bool, any Error>) -> Void) -> some View

Requests permission to save and read the specified HealthKit data types.

