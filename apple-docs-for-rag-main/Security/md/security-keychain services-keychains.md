

- Security
- Keychain services
-  Keychains 

API Collection

# Keychains

Create and manage entire keychains in macOS.

## Overview

In iOS, apps have access to a single keychain (which logically encompasses the iCloud keychain). This keychain is automatically unlocked when the user unlocks the device and then locked when the device is locked. An app can access only its own keychain items, or those shared with a group to which the app belongs. It can’t manage the keychain container itself.

In macOS, however, the system supports an arbitrary number of keychains. You typically rely on the user to manage these with the Keychain Access app and work implicitly with the default keychain, much as you would in iOS. Nevertheless, the keychain services API does provide functions that you can use to manipulate keychains directly. For example, you can create and manage a keychain that is private to your app. On the other hand, robust access control mechanisms typically make this unnecessary for anything other than an app trying to replicate the keychain access utility.

## Topics

### Creation and Deletion

func SecKeychainCreate(UnsafePointer&lt;CChar>, UInt32, UnsafeRawPointer?, Bool, SecAccess?, UnsafeMutablePointer&lt;SecKeychain?>) -> OSStatus

Creates an empty keychain.

Deprecated

func SecKeychainDelete(SecKeychain?) -> OSStatus

Deletes one or more keychains from the default keychain search list, and removes the keychain itself if it is a file.

Deprecated

class SecKeychain

An opaque type that represents a keychain.

func SecKeychainGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which a keychain object belongs.

Deprecated

### Locking and Unlocking

func SecKeychainLock(SecKeychain?) -> OSStatus

Locks a keychain.

Deprecated

func SecKeychainLockAll() -> OSStatus

Locks all keychains belonging to the current user.

Deprecated

func SecKeychainUnlock(SecKeychain?, UInt32, UnsafeRawPointer?, Bool) -> OSStatus

Unlocks a keychain.

Deprecated

### Settings

func SecKeychainSetSettings(SecKeychain?, UnsafePointer&lt;SecKeychainSettings>) -> OSStatus

Changes the settings of a keychain.

Deprecated

func SecKeychainCopySettings(SecKeychain?, UnsafeMutablePointer&lt;SecKeychainSettings>) -> OSStatus

Obtains a keychain’s settings.

Deprecated

struct SecKeychainSettings

A structure that contains information about keychain settings.

var SEC_KEYCHAIN_SETTINGS_VERS1: Int32

Defines the keychain settings version.

### Keychain Management

func SecKeychainGetVersion(UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Determines the version of keychain services installed on the user’s system.

Deprecated

func SecKeychainOpen(UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;SecKeychain?>) -> OSStatus

Opens a keychain.

Deprecated

func SecKeychainSetDefault(SecKeychain?) -> OSStatus

Sets the default keychain.

Deprecated

func SecKeychainCopyDefault(UnsafeMutablePointer&lt;SecKeychain?>) -> OSStatus

Retrieves a pointer to the default keychain.

Deprecated

func SecKeychainGetPath(SecKeychain?, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;CChar>) -> OSStatus

Determines the path of a keychain.

Deprecated

func SecKeychainGetStatus(SecKeychain?, UnsafeMutablePointer&lt;SecKeychainStatus>) -> OSStatus

Retrieves status information of a keychain.

Deprecated

typealias SecKeychainStatus

A value that defines the current status of a keychain.

SecKeychainStatus Values

Valid values for the keychain status type.

### Search

func SecKeychainSetSearchList(CFArray) -> OSStatus

Specifies the list of keychains to use in the default keychain search list.

Deprecated

func SecKeychainCopySearchList(UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves a keychain search list.

Deprecated

class SecKeychainSearch

An opaque type that contains information about a keychain search.

### User Interaction

func SecKeychainSetUserInteractionAllowed(Bool) -> OSStatus

Enables or disables the user interface for keychain services functions that automatically display a user interface.

Deprecated

func SecKeychainGetUserInteractionAllowed(UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Indicates whether keychain services functions that normally display a user interaction are allowed to do so.

Deprecated

### Callbacks

func SecKeychainAddCallback(SecKeychainCallback, SecKeychainEventMask, UnsafeMutableRawPointer?) -> OSStatus

Registers your keychain event callback function.

Deprecated

func SecKeychainRemoveCallback(SecKeychainCallback) -> OSStatus

Unregisters your keychain event callback function.

Deprecated

typealias SecKeychainCallback

A customized callback function that keychain services call when a keychain event has occurred.

Deprecated

struct SecKeychainCallbackInfo

Information about a keychain event that keychain services deliver to your app via a callback function.

enum SecKeychainEvent

The list of keychain events that can trigger a callback.

struct SecKeychainEventMask

Bit masks corresponding to the events that can trigger a keychain callback.

### Preference Domains

func SecKeychainGetPreferenceDomain(UnsafeMutablePointer&lt;SecPreferencesDomain>) -> OSStatus

Gets the current keychain preference domain.

Deprecated

func SecKeychainSetPreferenceDomain(SecPreferencesDomain) -> OSStatus

Sets the keychain preference domain.

Deprecated

func SecKeychainCopyDomainDefault(SecPreferencesDomain, UnsafeMutablePointer&lt;SecKeychain?>) -> OSStatus

Retrieves the default keychain from a specified preference domain.

Deprecated

func SecKeychainSetDomainDefault(SecPreferencesDomain, SecKeychain?) -> OSStatus

Sets the default keychain for a specified preference domain.

Deprecated

func SecKeychainCopyDomainSearchList(SecPreferencesDomain, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

Retrieves the keychain search list for a specified preference domain.

Deprecated

func SecKeychainSetDomainSearchList(SecPreferencesDomain, CFArray) -> OSStatus

Sets the keychain search list for a specified preference domain.

Deprecated

enum SecPreferencesDomain

The keychain preference domains.

### Access

func SecKeychainSetAccess(SecKeychain?, SecAccess) -> OSStatus

Sets the application access for a keychain.

Deprecated

func SecKeychainCopyAccess(SecKeychain?, UnsafeMutablePointer&lt;SecAccess?>) -> OSStatus

Retrieves the application access of a keychain.

Deprecated

