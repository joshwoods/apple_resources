

- ClassKit
- CLSDataStore
-  Building missing contexts 

Article

# Building missing contexts

Create and initialize missing contexts.

## Overview

When you request a context with a call to the descendant(matchingIdentifierPath:completion:) method, whether because you are declaring it or because you want to do something with it, the data store returns the context indicated by the identifier path. But if that context or any of its ancestors doesn’t already exist, the data store asks its delegate to create new ones.

### Adopt the data store delegate protocol

To enable the delegate to create a context, you adopt the CLSDataStoreDelegate protocol in your app.

```
```

The data store uses the delegate callback to ask for each new context it encounters. You use the identifier path to determine exactly what the new context should look like. A good way to do this is to map the identifier path to a model object you already have and use its properties to inform context creation. For example, your model objects might represent books, chapters, sections, and quizzes, all of which implement a `title` parameter suitable for use on the context. By also storing a `contextType` parameter on each model instance, with values like CLSContextType.book, CLSContextType.chapter, CLSContextType.section, or CLSContextType.quiz, you can create contexts based entirely on model instances, as shown above.

### Provide descriptive titles

The title you provide at context initialization is what teachers see when browsing your content in the Schoolwork app. Make it easy for teachers to understand what your app offers by choosing good context titles and localizing them, as appropriate. Because titles are the most visible aspect of your hierarchy, it’s important that you make them both clear and descriptive. The title “Thermodynamics Quiz” is much more self-explanatory than “Quiz 8” for example.

### Optionally, indicate display order

If appropriate, provide guidance for ordering your contexts using the displayOrder property. For example, immediately after instantiating a context that represents a chapter, you might indicate its position as the chapter number:

```
```

### Classify contexts by subject

You can further classify a context with an optional topic using one of the values from CLSContextTopic, like math or socialScience. For apps covering a variety of different subject matters, topics help teachers differentiate between the various parts of your app. An app that has a singular focus can simply set its top-level context to the topic that best matches that subject. For example, for a book reader:

```
```

### Return the context

Once you create and configure the context, you simply return it to the data store. The data store associates the context with the appropriate parent and keeps it in memory. The next time you ask the data store for that context, it returns the previously generated one instead of requesting a new one from the delegate. Additionally, for a user logged in as a teacher, the data store saves the changes to an internal database that’s shared with the Schoolwork app and synchronized over iCloud. This allows the context to persist even across launches of your app, but only for teachers. For privacy reasons, other users don’t record contexts in the database.

Note

It’s possible to build a context hierarchy without using the delegate protocol by initializing CLSContext instances and manually assigning them as children of other contexts, starting with the app’s main context at the root. But a context hierarchy might already exist in the local data store from a previous launch of your app. Rebuilding generates needless network traffic while the updates are synchronized through iCloud. By using a data store delegate, you only create new contexts when they aren’t already in the data store.

## See Also

### Managing the delegate

var delegate: (any CLSDataStoreDelegate)?

The data store delegate instance.

protocol CLSDataStoreDelegate

An interface the data store uses to request new contexts.

