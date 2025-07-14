

- Dispatch
-  Dispatch Objects 

API Collection

# Dispatch Objects

The basic behaviors supported by all dispatch types.

## Overview

There are many types of dispatch objects, including dispatch_queue_t, dispatch_group_t, and dispatch_source_t. The base dispatch object interfaces allow you to manage memory, pause and resume execution, define object context, log task data, and more.

By default, dispatch objects are declared as Objective-C types when you build them with an Objective-C compiler. This behavior lets you adopt ARC and enable memory leak checks by the static analyzer. It also lets you add your objects to Cocoa collections.

## Topics

### Activating, Suspending, and Resuming the Object

func activate()

Activates the dispatch object.

func suspend()

Suspends the invocation of block objects on a dispatch object.

func resume()

Resumes the invocation of block objects on a dispatch object.

typealias dispatch_object_t

A dispatch object.

### Changing the Assigned Target Queue

func setTarget(queue: dispatch_queue_t?)

Specifies the dispatch queue on which to perform work associated with the current object.

## See Also

### Dispatch Objects

class DispatchObject

The base class for most dispatch types.

enum DispatchPredicate

Logical conditions to evaluate within a given execution context.

func dispatchPrecondition(condition: @autoclosure () -> DispatchPredicate)

Checks a dispatch condition necessary for further execution.

