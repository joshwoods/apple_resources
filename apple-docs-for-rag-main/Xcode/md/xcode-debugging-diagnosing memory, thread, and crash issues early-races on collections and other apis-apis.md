

- Xcode
- Debugging
- Diagnosing memory, thread, and crash issues early
-  Races on collections and other APIs 

Article

# Races on collections and other APIs

Detects when one thread accesses a mutable object while another thread is writing to it.

## Overview

In Xcode 9 and later, the Thread Sanitizer detects unsafe thread accesses of Foundation and Core Foundation framework APIs. This feature applies to the following collection types:

- NSMutableArray

- NSMutableDictionary

- CFMutableArray

- CFMutableDictionary

### Collection race with a mutable array

In the following example, the code enumerates a mutable array in one thread while writing to the array from another without synchronizing access:

**Swift**

```
let array: NSMutableArray = []
var sum: Int = 0
// Executed on Thread #1
for value in array {
    sum += value as! Int
}
// Executed on Thread #2
array.add(42)
```

**Objective-C**

```
NSMutableArray *array = [NSMutableArray new];
NSInteger sum = 0;
// Executed on Thread #1
for (id value in array) {  
    sum += [value integerValue];
} 
// Executed on Thread #2
[array addObject:@42];
```

#### Solution

Use Dispatch APIs to coordinate access to `array` across multiple threads.

### Collection race with a mutable dictionary

In the following example, the code enumerates a mutable dictionary in one thread while writing to the dictionary from another without synchronizing access:

```
let dictionary: NSMutableDictionary = [:]
var sum: Int = 0
// Executed on Thread #1
for key in dictionary.keyEnumerator() {
    sum += dictionary[key] as! Int
}
// Executed on Thread #2
dictionary["forty-two"] = 42
```

**Objective-C**

```
NSMutableDictionary *dictionary = [NSMutableDictionary new];
NSInteger sum = 0;
// Executed on Thread #1
for (id key in dictionary) {
    sum += [dictionary[key] integerValue];
}
// Executed on Thread #2
dictionary[@"forty-two"] = @42;
```

#### Solution

Use Dispatch APIs to coordinate access to `dictionary` across multiple threads.

## See Also

### Thread Sanitizer

Data races

Detects unsynchronized access to mutable state across multiple threads.

Swift access races

Detects unsynchronized access to mutable state across multiple threads in Swift.

Uninitialized mutexes

Detects when you use an uninitialized mutex.

Thread leaks

Detects when you don’t close threads after use.

