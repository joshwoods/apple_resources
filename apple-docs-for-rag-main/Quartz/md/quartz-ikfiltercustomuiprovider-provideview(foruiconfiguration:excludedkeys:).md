

- Quartz
- IKFilterCustomUIProvider
-  provideView(forUIConfiguration:excludedKeys:) 

Instance Method

# provideView(forUIConfiguration:excludedKeys:)

Provides a custom view for a filter.

macOS 10.4+

``` source
func provideView(
    forUIConfiguration inUIConfiguration: [AnyHashable : Any]!,
    excludedKeys inKeys: [Any]!
) -> IKFilterUIView!
```

**Required**

## Parameters 

`inUIConfiguration`  

A dictionary that specifies the size of the controls. Provide the key `IKUISizeFlavor` and one of the following values: `IKUISizeMini`, `IKUISizeSmall`, or `IKUISizeRegular`. For more information on these constants, see *User Interface Options* in CIFilter Image Kit Additions.

`inKeys`  

An array of the input keys for which you do *not* want to provide a user interface. Pass `nil` if you want all input keys to be represented in the user interface.

## Return Value

An IKFilterUIView object or `nil` if the filter is unable to provide a view. If `nil`, the Image Kit framework will attempt to provide a user interface.

## Discussion

This method overrides the method view(forUIConfiguration:excludedKeys:).

