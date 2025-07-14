

- Bundle Resources
- Information Property List
-  ENAPIVersion 

Property List Key

# ENAPIVersion

A number that specifies the version of the API to use.

iOS 13.7+iPadOS 13.7+

## Details 

Type  

number

## Possible Values 

`1`  

Use version 1 of the API.

`2`  

Use version 2 of the API.

## Attributes 

Default: `1`

## Discussion

Important

This type is available in iOS 12.5, and in iOS 13.7 and later.

iOS 13.7 introduces a new method to calculate the user’s Exposure Risk Value, described in ENExposureConfiguration. Set this value to `2` to use this new version and its calculation method, or set this value to `1` to use the earlier API and its calculation method. If you don’t explicitly set this value, the default is `1`.

## See Also

### Exposure notification

ENDeveloperRegion

A string that specifies the region that the app supports.

