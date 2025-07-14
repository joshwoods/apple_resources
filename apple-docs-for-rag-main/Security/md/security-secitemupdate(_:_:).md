

- Security
-  SecItemUpdate(\_:\_:) 

Function

# SecItemUpdate(\_:\_:)

Modifies items that match a search query.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecItemUpdate(
    _ query: CFDictionary,
    _ attributesToUpdate: CFDictionary
) -> OSStatus
```

## Parameters 

`query`  

A dictionary that describes the search for the keychain items you want to update. A typical `query` dictionary consists of:

- **The item’s class.** Specify the kind of item you want, for example a password, a certificate, or a cryptographic key, using one of the class values in Item class keys and values.

- **Attributes.** Narrow the search by indicating the attributes that the found item or items should have. The more attributes you specify, the more refined the results, but not all attributes apply to all item classes. For the attributes applicable to the keychain item you’re updating, see the entry for the item’s class in Item class values.

- **Search parameters.** Condition the search in a variety of ways. For example, you can limit the results to a specific number of items, control case sensitivity when matching string attributes, or search only among a particular set of items. See Search attribute keys and values for the complete list of possible search parameters.

`attributesToUpdate`  

A dictionary containing the attributes whose values should update, along with the new values. Only real keychain attributes are permitted in this dictionary (no “meta” attributes are allowed.) For the attributes applicable to the keychain item you’re updating, see the entry for the item’s class in Item class values.

## Return Value

A result code. See Security Framework Result Codes.

## Mentioned in 

Updating and deleting keychain items

## Discussion

The query dictionary for update can’t contain Item return result keys, because SecItemUpdate(_:_:) only returns a status.

### Performance considerations

`SecItemUpdate` blocks the calling thread, so it can cause your app’s UI to hang if called from the main thread. Instead, call `SecItemUpdate` from a background dispatch queue or `async` function:

- Swift
- Objective-C

```
private func updateKeychainItem(searchAttributes attrs: CFDictionary, update updateAttrs: CFDictionary, _ completion: @escaping (OSStatus) -> Void) {
    queue.async {
        let result = SecItemUpdate(attrs, updateAttrs)
        completion(result)
    }
}

```

```
- (void)updateKeyChainItemWithAttributes:(CFDictionaryRef)attrs update:(CFDictionaryRef)update completion:(void(^)(OSStatus status))completion {
    dispatch_async(backgroundQueue, ^{
        OSStatus updateResult = SecItemUpdate(attrs, update);
        completion(updateResult);
    });
}
```

