

- HIDDriverKit
- IOHIDElement
-  conformsTo 

Instance Method

# conformsTo

DriverKit 21.0+macOS

``` source
bool conformsTo(uint32_t usagePage, uint32_t usage);
```

## Parameters 

`usagePage`  

The usage page to check for conformity.

`usage`  

The usage to check for conformity.

## Return Value

Returns a bool specifying if the element conforms to the provided usage page and usage.

## Discussion

Checks if the element conforms to the provided usage page and usage somewhere in its hierarchy.

