

- Kernel
- Kernel Enumerations
- Anonymous
-  kIOFWMustHaveGap63 

Enumeration Case

# kIOFWMustHaveGap63

macOS 10.12+

``` source
kIOFWMustHaveGap63 = (1 

## Discussion

Attempt to ensure the gap count is 63, when this device is on the bus. Gap 63 reduces bus performance significantly, so this flag should be used only when absolutely necessary. There is no guarentee Mac OS will succeed in forcing the gap count to 63.

