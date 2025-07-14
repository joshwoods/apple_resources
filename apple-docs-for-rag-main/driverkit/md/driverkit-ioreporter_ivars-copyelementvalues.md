

- DriverKit
- IOReporter_IVars
-  copyElementValues 

Instance Method

# copyElementValues

DriverKitiOSiPadOSmacOS

``` source
IOReturn copyElementValues(int element_index, IOReportElementValues * elementValues);
```

## Parameters 

`element_index`  

- Index of the element to return values from

`elementValues`  

- For returning the content of element values

## Return Value

Returns the content of an element

## Discussion

For efficiently and thread-safely reading \_elements. May need to find the index of the element first.

Locking: Caller must ensure that the reporter (data) lock is held.

