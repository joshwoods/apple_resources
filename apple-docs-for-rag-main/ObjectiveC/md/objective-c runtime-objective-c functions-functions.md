

- Objective-C Runtime
-  Objective-C Functions 

API Collection

# Objective-C Functions

## Topics

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

func objc_exception_throw(Any) -> Never

Throw a runtime exception. This function is inserted by the compiler where \c @throw would otherwise be.

func objc_finalizeOnMainThread(AnyClass!)Deprecated

func objc_is_finalized(UnsafeMutableRawPointer!) -> BoolDeprecated

func objc_memmove_collectable(UnsafeMutableRawPointer!, UnsafeRawPointer!, Int) -> UnsafeMutableRawPointer!Deprecated

func objc_registerThreadWithCollector()Deprecated

func objc_removeExceptionHandler(UInt)

func objc_set_collection_ratio(Int)Deprecated

func objc_set_collection_threshold(Int)Deprecated

func objc_setCollectionRatio(Int)Deprecated

func objc_setCollectionThreshold(Int)Deprecated

func objc_setExceptionMatcher(objc_exception_matcher) -> objc_exception_matcher

func objc_setExceptionPreprocessor(objc_exception_preprocessor) -> objc_exception_preprocessor

func objc_setForwardHandler(UnsafeMutableRawPointer, UnsafeMutableRawPointer)

Set the function to be called by objc_msgForward.

func objc_setHook_getClass(objc_hook_getClass, UnsafeMutablePointer&lt;objc_hook_getClass?>)

func objc_setHook_getImageName(objc_hook_getImageName, UnsafeMutablePointer&lt;objc_hook_getImageName?>)

func objc_setHook_lazyClassNamer(objc_hook_lazyClassNamer, UnsafeMutablePointer&lt;objc_hook_lazyClassNamer>)

func objc_setUncaughtExceptionHandler(objc_uncaught_exception_handler) -> objc_uncaught_exception_handler

func objc_start_collector_thread()Deprecated

func objc_startCollectorThread()Deprecated

func objc_sync_enter(Any) -> Int32

Begin synchronizing on ‘obj’.  
Allocates recursive pthread_mutex associated with ‘obj’ if needed.

func objc_sync_exit(Any) -> Int32

End synchronizing on ‘obj’.

func objc_terminate() -> Never

func objc_unregisterThreadWithCollector()Deprecated

func object_isClass(Any?) -> Bool

func object_setIvarWithStrongDefault(Any?, Ivar, Any?)

func protocol_copyPropertyList2(Protocol, UnsafeMutablePointer&lt;UInt32>?, Bool, Bool) -> UnsafeMutablePointer&lt;objc_property_t>?

func sel_isMapped(Selector) -> Bool

Identifies a selector as being valid or invalid.

## See Also

### Reference

Objective-C Runtime

Describes the macOS Objective-C runtime library support functions and data structures.

Objective-C Structures

Objective-C Constants

Objective-C Data Types

Objective-C Macros

Objective-C Enumerations

