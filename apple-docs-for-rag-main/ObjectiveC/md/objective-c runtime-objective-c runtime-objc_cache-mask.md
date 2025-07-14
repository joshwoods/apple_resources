

- Objective-C Runtime
- Objective-C Runtime
- objc_cache
-  mask 

Article

# mask

An integer specifying the total number of allocated cache buckets (minus one). During method lookup, the Objective-C runtime uses this field to determine the index at which to begin a linear search of the `buckets` array. A pointer to a method’s selector is masked against this field using a logical AND operation (`index = (mask & selector))`. This serves as a simple hashing algorithm.

## See Also

### Fields

occupied

An integer specifying the total number of occupied cache buckets.

buckets

An array of pointers to Method data structures. This array may contain no more than `mask + 1` items. Note that pointers may be `NULL`, indicating that the cache bucket is unoccupied, and occupied buckets may not be contiguous. This array may grow over time.

