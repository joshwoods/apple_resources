

- Core Services
- File Metadata
-  MDQuery 

API Collection

# MDQuery

## Overview

MDQuery is a CF-compliant object, follows the CF conventions,and can be used with the CF polymorphic functions, such as `CFRetain`.MDQuery encapsulates queries against the System store of the filemetadata.

An MDQuery normally executes asynchronously and posts progressnotifications as the results are collected. During the gatheringphase the query results conform to the specified value lists andsorting.

MDQuery gathers results and processes updates only while thecurrent thread's run loop is running.

For functions that take an MDQueryRef parameter, if this parameteris not a valid MDQueryRef, the behavior is undefined. `NULL` isnot a valid MDQueryRef.

For functions that take CF\*Ref parameters, such as CFStringRefand CFArrayRef, if this parameter is not a valid CF object of thecorrect type, the behavior is undefined. `NULL` isnot a valid CF\*Ref.

## Topics

### Creating Queries

func MDQueryCreate(CFAllocator!, CFString!, CFArray!, CFArray!) -> MDQuery!

Creates a new query instance.

func MDQueryCreateSubset(CFAllocator!, MDQuery!, CFString!, CFArray!, CFArray!) -> MDQuery!

Creates a new query that is a subset of the specified parentquery.

func MDQuerySetSearchScope(MDQuery!, CFArray!, OptionBits)

Sets the search scope for a query instance.

func MDQuerySetDispatchQueue(MDQuery!, dispatch_queue_t!)

Sets the dispatch queue on which query results will be delivered by MDQueryExecute.

### Getting and Setting Query Parameters

func MDQuerySetMaxCount(MDQuery!, CFIndex)

Sets the maximum number of results returned.

func MDQueryGetBatchingParameters(MDQuery!) -> MDQueryBatchingParams

Returns the current parameters that control the batching of progress notifications.

func MDQuerySetBatchingParameters(MDQuery!, MDQueryBatchingParams)

Set the query batching parameters.

func MDQueryCopyValueListAttributes(MDQuery!) -> CFArray!

Returns the list of attribute names for which values are being collected by the query.

func MDQueryCopySortingAttributes(MDQuery!) -> CFArray!

Returns the list of attribute names used to sort the results.

func MDQueryCopyQueryString(MDQuery!) -> CFString!

Returns the query string of the query.

### Setting Callback Functions

func MDQuerySetCreateResultFunction(MDQuery!, MDQueryCreateResultFunction!, UnsafeMutableRawPointer!, UnsafePointer&lt;CFArrayCallBacks>!)

Sets the function used to create the result objects of the MDQuery.

func MDQuerySetSortComparator(MDQuery!, MDQuerySortComparatorFunction!, UnsafeMutableRawPointer!)

Sets the function used to sort the results of an MDQuery.

func MDQuerySetCreateValueFunction(MDQuery!, MDQueryCreateValueFunction!, UnsafeMutableRawPointer!, UnsafePointer&lt;CFArrayCallBacks>!)

Sets the function used to create the value objects of the MDQuery.

### Starting, Stopping and Pausing Queries

func MDQueryExecute(MDQuery!, CFOptionFlags) -> Bool

Run the query, and populate the query with the results.

func MDQueryStop(MDQuery!)

Stops the query from generating more results.

func MDQueryDisableUpdates(MDQuery!)

Disables updates to the query result list.

func MDQueryEnableUpdates(MDQuery!)

Enables updates to the query result list.

func MDQueryIsGatheringComplete(MDQuery!) -> Bool

Returns true if the first phase of a query, the initial result gathering, has finished.

### Getting Query Result Values

func MDQueryCopyValuesOfAttribute(MDQuery!, CFString!) -> CFArray!

Returns the list of values from the results of the query for the specified attribute.

func MDQueryGetAttributeValueOfResultAtIndex(MDQuery!, CFString!, CFIndex) -> UnsafeMutableRawPointer!

Returns the value of the named attribute for the result at the given index.

func MDQueryGetCountOfResultsWithAttributeValue(MDQuery!, CFString!, CFTypeRef!) -> CFIndex

Returns the number of results which have the given attribute and attribute value.

func MDQueryGetIndexOfResult(MDQuery!, UnsafeRawPointer!) -> CFIndex

Returns the current index of the given result.

func MDQueryGetResultAtIndex(MDQuery!, CFIndex) -> UnsafeRawPointer!

Returns the current result at the given index.

func MDQueryGetResultCount(MDQuery!) -> CFIndex

Returns the number of results currently collected by the query.

func MDQuerySetSortComparatorBlock(MDQuery!, ((UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?, UnsafePointer&lt;Unmanaged&lt;CFTypeRef>?>?) -> CFComparisonResult)!)

Sets the block used to sort the results of an MDQuery.

### Getting the Type Identifier

func MDQueryGetTypeID() -> CFTypeID

Returns the type identifier of all MDQuery instances

### Callbacks

typealias MDQuerySortComparatorFunction

Callback function used to sort the results of a query.

typealias MDQueryCreateResultFunction

Callback function used to create the result objects stored and returned by a query.

typealias MDQueryCreateValueFunction

Callback function usedto create the value objects stored and returned by a query.

### Batching Parameters

struct MDQueryBatchingParams

Structure containing the progress notification batchingparameters of a MDQuery.

### Miscellaneous

class MDQuery

A reference to a MDQuery object.

### Query Option Flags

struct MDQueryOptionFlags

Specify the execution mode for a query.

### Notifications

kMDQueryDidFinishNotification

Indicates that a query has finished with the initial result-gathering phase.

kMDQueryDidUpdateNotification

Indicates that a query’s results list has change during the live-update phase of a query.

kMDQueryProgressNotification

Indicates that a query’s results list has change during the initial result-gathering phase of a query.

### Notification Info Keys

Query Result Change Keys

Specify the items that have changed in the query results.

Query Search Scope Keys

Specify the scope of a query’s search.

Result Relevance Sorting Key

Key used in a user notification’s description dictionary that indicates the relevance of a result.

## See Also

### Related Documentation

Spotlight Overview

File Metadata Search Programming Guide

