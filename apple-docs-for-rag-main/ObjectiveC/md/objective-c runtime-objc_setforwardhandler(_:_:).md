

- Objective-C Runtime
-  objc_setForwardHandler(\_:\_:) 

Function

# objc_setForwardHandler(\_:\_:)

Set the function to be called by objc_msgForward.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_setForwardHandler(
    _ fwd: UnsafeMutableRawPointer,
    _ fwd_stret: UnsafeMutableRawPointer
)
```

## Parameters 

`fwd`  

Function to be jumped to by objc_msgForward.

`fwd_stret`  

Function to be jumped to by objc_msgForward_stret.

## See Also

### Functions

func autoreleasepool&lt;E, Result>(invoking: () throws(E) -> Result) throws(E) -> Result

func class_lookupMethod(AnyClass?, Selector) -> IMP?Deprecated

func class_respondsToMethod(AnyClass?, Selector) -> BoolDeprecated

func objc_addExceptionHandler(objc_exception_handler, UnsafeMutableRawPointer?) -> UInt

func objc_addLoadImageFunc(objc_func_loadImage)

func objc_assertRegisteredThreadWithCollector()Deprecated

func objc_begin_catch(UnsafeMutableRawPointer) -> Any

func objc_clear_stack(UInt)Deprecated

func objc_collect(UInt)Deprecated

func objc_collectableZone() -> objc_zone_t!Deprecated

func objc_collecting_enabled() -> BoolDeprecated

func objc_collectingEnabled() -> BoolDeprecated

func objc_end_catch()

func objc_enumerateClasses(fromImage: ObjCEnumerationImage, matchingNamePrefix: String?, conformingTo: Protocol?, subclassing: AnyClass?) -> ObjCClassList

func objc_exception_rethrow() -> Never

