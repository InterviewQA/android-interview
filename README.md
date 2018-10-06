<h1 align="center">Android Interview Questions</h1>

## Table of Contents

1. [Core Java or Kotlin](#core-java-or-kotlin-questions)
1. [Core Android](#core-android-questions)
1. [Design](#design-questions)
1. [Data Storage](#data-storage-questions)
1. [Architecture](#architecture-questions)
1. [Tools and Libraries](#tools-and-libraries-questions)
1. [Test Driven Development](#test-driven-development-questions)
1. [Others](#others-questions)

# Core Java or Kotlin Questions
* [What is overloading and overriding in java?](#what-is-overloading-and-overriding-in-java)

# Core Android Questions
* [What is difference between Serializable and Parcelable ? Which is best approach in Android ?]()

# Design Questions

# Data Storage Questions

# Architecture Questions

# Tools and Libraries Questions

# Other Questions





### What is overloading and overriding in java?

When we have more than one method with the same name in a single class but the arguments are different, then it is called as method overloading.

Overriding concept comes in picture with inheritance when we have two methods with same signature, one in parent class and another in child class. We can use `@Override` annotation in the child class overridden method to make sure if parent class method is changed, so as child class.

###### References

* https://www.journaldev.com/2366/core-java-interview-questions-and-answers#java-oops

[[↑] Back to top](#core-java-or-kotlin-questions)

### What is difference between Serializable and Parcelable ? Which is best approach in Android ?

`Serializable` is a standard Java interface. You simply mark a class Serializable by implementing the interface, and Java will automatically serialize it in certain situations.

`Parcelable` is an Android specific interface where you implement the serialization yourself. It was created to be far more efficient than Serializable, and to get around some problems with the default Java serialization scheme.

###### References

* https://www.toptal.com/android/interview-questions

[[↑] Back to top](#core-android)

## Translations

* [English](/README.md)


## Contributing
You should make sure your question/answer is appropriate and unique for this repository and if you don't know how to contribute, you should read [CONTRIBUTING](/CONTRIBUTING) guide before pull request.

## License

All projects and packages in this repository are [MIT licensed](/LICENSE).
