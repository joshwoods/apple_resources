

- HIDDriverKit
- IOUserHIDEventService
-  conformsTo 

Instance Method

# conformsTo

Returns a Boolean value that indicates whether the service conforms to the specified HID usage and page information.

DriverKit 19.0+macOS

``` source
bool conformsTo(uint32_t usagePage, uint32_t usage);
```

## Parameters 

`usagePage`  

The HID usage page value.

`usage`  

The HID usage value from the specified page.

## Return Value

`true` if the service conforms to the specified usage and page information, or `false` if it doesn’t.

## Discussion

Use this method to determine if a service is able to provide the specified type of data. This method iterates over the properties of the service’s provider object to look for the specified usage and page information, returning `true` if it finds an exact match.

