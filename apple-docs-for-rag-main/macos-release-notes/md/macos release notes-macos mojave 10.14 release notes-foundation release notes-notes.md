

- macOS Release Notes
- macOS Mojave 10.14 Release Notes
-  Foundation Release Notes 

Article

# Foundation Release Notes

Update your apps to use new features, and test your apps against API changes.

## Overview

Foundation in macOS 10.14, iOS 12, watchOS 5, and tvOS 12 includes new features, API changes, and deprecations. For information about earlier releases, see Foundation Release Notes for macOS 10.13 and iOS 11.

### Secure Data Archival and Unarchival

The NSKeyedArchiver and NSKeyedUnarchiver classes have new initializers and helper methods that make it easier for you to enable secure coding for archival and unarchival. Each initializer or helper method replaces a corresponding member that’s now deprecated.

- init(requiringSecureCoding:) replaces init() and init(forWritingWith:).

- archivedData(withRootObject:requiringSecureCoding:) replaces archivedData(withRootObject:) and archiveRootObject(_:toFile:).

- init(forReadingFrom:) replaces init() and init(forReadingWith:).

- unarchivedObject(ofClass:from:) and unarchivedObject(ofClasses:from:) replace unarchiveObject(with:), unarchiveTopLevelObjectWithData(_:), and unarchiveObject(withFile:).

You use the new unarchivedObject(ofClasses:from:) method when unarchiving instances that are subclasses of one of the list of classes you supply. You can use these initializers and helper methods in apps that are compatible with macOS 10.13, iOS 11, watchOS 4, tvOS 11, and subsequent releases of each operating system.

For more information, see the WWDC 2018 session Data You Can Trust.

### Secure Value Transformer

NSSecureUnarchiveFromDataTransformer is a new subclass of ValueTransformer. It uses NSKeyedArchiver and NSKeyedUnarchiver to archive and unarchive data by enabling requiresSecureCoding.

When unarchiving from NSData, NSSecureUnarchiveFromDataTransformer uses its allowedTopLevelClasses list to decode objects by calling the new unarchivedObject(ofClasses:from:) method. By default, this list includes all property list types—NSArray, NSDictionary, NSString, NSNumber, NSDate, NSData, and NSNull—along with NSURL and NSUUID.

When archiving to NSData, this transformer calls the new archivedData(withRootObject:requiringSecureCoding:) method and enables requiresSecureCoding.

To transform top-level values of types other than the defaults listed above, subclass NSSecureUnarchiveFromDataTransformer.

- If you expect to decode a top-level value of only one allowed type, override transformedValueClass() to return that type. Doing so populates allowedTopLevelClasses automatically.

- If you expect to decode a top-level value of one of several allowed types, override allowedTopLevelClasses to return those types.

The older unarchiveFromDataTransformerName and keyedUnarchiveFromDataTransformerName values are now deprecated.

### NSSecureCoding Conformance

The NSPointerFunctions, NSMapTable, and NSHashTable classes now support limited conformance to the NSSecureCoding protocol. You can securely encode pointer-function consuming collections as long as you configure them with the following personalities and kinds of memory:

- objectPersonality

- objectPointerPersonality

- strongMemory

- weakMemory

- copyIn (optional)

Important

Weak values won’t round-trip as expected unless you strongly reference them elsewhere during unarchival.

### Macro for Closed Enumerations

`NS_CLOSED_ENUM` is a new macro for declaring enumerations. You use it only for enumerations that are guaranteed to never gain an additional case. Usually you determine that there won’t be new cases because the enumeration you’re modeling represents a mathematically complete set. ComparisonResult now adopts the `NS_CLOSED_ENUM` macro. It won’t ever gain additional cases.

Important

Once an enumeration is marked as closed, it’s a binary- and source-incompatible change to add a new value. If you have any doubt about an enumeration gaining a private or additional public case in the future, use the `NS_ENUM` macro instead.

For information about `NS_CLOSED_ENUM` and choosing between it and other macros for grouping constants, see Grouping Related Objective-C Constants.

### UserDefaults

UserDefaults has several bug fixes and improvements:

- Removed synchronization requirements. It’s no longer necessary to use synchronize(), CFPreferencesAppSynchronize(_:), or CFPreferencesSynchronize(_:_:_:). These methods will be deprecated in a future version of the OS.Now that you don’t need to call these synchronization methods, the performance characteristics of UserDefaults and Preferences Utilities are slightly different: The time taken for enqueueing write operations is now paid by the writing thread, rather than by the next thread to call synchronize() or do a read operation.

- Removed retains when adding an observer. Adding observers to an instance of UserDefaults using the addObserver(_:forKeyPath:options:context:) method unintentionally retained it, unlike all other uses of key-value observing. This has been corrected, and normal Cocoa memory management rules are now followed.

- Fixed key-value observing bug in UserDefaults. Reading defaults on one thread while another thread set defaults could nondeterministically send key-value observing notifications on both threads, rather than just the thread doing the set operation. This is now fixed.

### On-Demand Resources

NSBundleResourceRequest no longer throws exceptions when encountering certain kinds of internal errors. Instead, it returns an error in the error argument of the completion handler of the beginAccessingResources(completionHandler:) method. The error might include the NSFileReadUnknownError and NSXPCConnectionInterrupted errors in addition to NSUserCancelledError and network-related errors.

If your app encounters an error when using NSBundleResourceRequest, request the resource again or display a prompt to your user to try again.

### Thread Safety of Bundles

The principalClass property on Bundle includes new thread-safety improvements. Accessing the property blocks if other threads are in the process of loading the bundle. This action allows the property to return the correct value in all cases.

### CFMessagePort

The CFMessagePortSetName(_:_:) function doesn’t do anything in apps linked on or after macOS 10.14, iOS 12, watchOS 5, and tvOS 12. This API will be deprecated in a future release.

In apps linked on earlier versions of macOS, iOS, watchOS, and tvOS, the CFMessagePortSetName(_:_:) function doesn’t do anything if the message port already has a dispatch queue associated with itself via the CFMessagePortSetDispatchQueue(_:_:) function. Previously, this pattern would result in undefined behavior.

In all cases, if you need to change the name of a CFMessagePort, use CFMessagePortCreateLocal(_:_:_:_:_:) or CFMessagePortCreateRemote(_:_:).

