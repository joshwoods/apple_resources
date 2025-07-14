

- PencilKit
- PKToolPicker
-  removeObserver(\_:) 

Instance Method

# removeObserver(\_:)

Removes the specified object from the list of objects to notify when the picker configuration changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func removeObserver(_ observer: any PKToolPickerObserver)
```

## Parameters 

`observer`  

The object to stop sending notifications to.

## See Also

### Detecting changes to the picker

func addObserver(any PKToolPickerObserver)

Adds the specified object to the list of objects to notify when the picker configuration changes.

protocol PKToolPickerObserver

An interface you use to detect when the user changes the selected tools and drawing characteristics of a tool picker object.

