# Android Interview Questions

> A curated collection of Android interview questions and answers

## Table of Contents

1. [Core Java or Kotlin](#core-java-or-kotlin-questions)
1. [Core Android](#core-android-questions)
1. [Design](#design-questions)
1. [Data Storage](#data-storage-questions)
1. [Architecture](#architecture-questions)
1. [Tools and Libraries](#tools-and-libraries-questions)
1. [Test Driven Development](#test-driven-development-questions)
1. [Others](#others-questions)

## Core Java or Kotlin Questions
* [What is overloading and overriding in java?](#what-is-overloading-and-overriding-in-java)

## Core Android Questions
* [What is difference between `Serializable` and `Parcelable`? Which is best approach in Android?](#what-is-difference-between-serializable-and-parcelable-which-is-best-approach-in-android)
* [What is the difference between `Service` and `IntentService`? How is each used?](#what-is-the-difference-between-service-and-intentservice-how-is-each-used)

## Design Questions

## Data Storage Questions
* [What are the different data storage options available on the Android platform?]()

## Architecture Questions

## Tools and Libraries Questions

## Other Questions





### What is overloading and overriding in java?

When we have more than one method with the same name in a single class but the arguments are different, then it is called as method overloading.

Overriding concept comes in picture with inheritance when we have two methods with same signature, one in parent class and another in child class. We can use `@Override` annotation in the child class overridden method to make sure if parent class method is changed, so as child class.

###### References

* https://www.journaldev.com/2366/core-java-interview-questions-and-answers#java-oops

[[↑] Back to top](#core-java-or-kotlin-questions)

### What is difference between `Serializable` and `Parcelable`? Which is best approach in Android?

`Serializable` is a standard Java interface. You simply mark a class Serializable by implementing the interface, and Java will automatically serialize it in certain situations.

`Parcelable` is an Android specific interface where you implement the serialization yourself. It was created to be far more efficient than Serializable, and to get around some problems with the default Java serialization scheme.

###### References

* https://www.toptal.com/android/interview-questions

[[↑] Back to top](#core-android-questions)


### What is the difference between `Service` and `IntentService?`? How is each used?

`Service`: It is the base class for the Android services, that you can extend for creating any service. Since the service run inside the UI thread, it requires that you create a working thread for executing its work.

`IntentService`: it is a subclass of Service, that simplifies your work. It works already in a working thread, and can receive asynchronous requests. So, you don't need to create it manually, or to worry about synchronization. You can simply extend it and override the method `onHandleIntent(Intent intent)`

IntentService do for you:
- Creates a default worker thread that executes all intents delivered to `onStartCommand()` separate from your application's main thread.
- Creates a work queue that passes one intent at a time to your `onHandleIntent()` implementation, so you never have to worry about multi-threading.
- Stops the service after all start requests have been handled, so you never have to call `stopSelf()`
- Provides default implementation of `onBind()` that returns null.
- Provides a default implementation of `onStartCommand()` that sends the intent to the work queue and then to your `onHandleIntent()` implementation.

###### References

* https://stackoverflow.com/questions/31451476/what-is-the-difference-between-service-intentservice-in-android

[[↑] Back to top](#core-android-questions)


### What are the different data storage options available on the Android platform?
**SharedPreference:** It stores data in XML files. It is the simplest way to store private data in the key-value pair.  
**SQLite:** It stores structure data in the private database.  
**Internal Storage:** It stores data in the device file system and any other app cannot read this data.  
**External Storage:** Data is stored in the file system but it is accessible to all apps in the device  

###### References
* https://developer.android.com/guide/topics/data/data-storage

[[↑] Back to top](#data-storage-questions)

## Translations

* [English](/README.md)


## Contributing
You should make sure your question/answer is appropriate and unique for this repository and if you don't know how to contribute, you should read [CONTRIBUTING](/CONTRIBUTING) guide before pull request.

## License

All projects and packages in this repository are [MIT licensed](/LICENSE).
