---
title: "Object Oriented Programming (OOP)"
description: "Introduction to object-oriented programming and its key concepts"
date: "2022-08-07 17:00:00 +05:30"

author: "Siddharth Arumugam"
tags: ["programming", "object-oriented-programming"]
aliases: oop
---

## What is object oriented programming?

Object-oriented programming (OOP) is a programming paradigm (style of programming) based on [objects](#object).

Some programming languages based on OOP are Java, C++, JavaScript, Python, etc.

## OOP Terms

Let us first learn some of the key terms used in OOP.

#### Method
Member function of a class. Each method contains a method signature which comprises of the method name and method parameter types.

#### State
Member variable of a class, accessible by its methods.

#### Class
A class is a user-defined data type that is a template for an object.
The class provides the initial values for state and contains methods.

#### Object
An object is an instance of a class. It is a combination of variables and methods.

## Basic principles of OOP

Object-oriented programming encompasses four basic principles: [Data Abstraction](#data-abstraction), [Inheritance](#inheritance), [Encapsulation](#encapsulation), [Polymorphism](#polymorphism).

#### Data Abstraction

Data abstraction refers to showing only essential information to the user, while hiding the underlying implementation details.

For example, we are able to dial a phone number and make a call. However, we don't know the internal working of the phone and how the signals are transmitted.

#### Inheritance

Inheritance is the process by which a class (subclass) acquires the properties of another class (superclass). The subclass gets all the features of the base class and can have its own.

> The _subclass_ is also called the _derived/extended/child_ class.\
> The _superclass_ is also called the _base/parent_ class.

#### Encapsulation

Encapsulation implements data hiding by restricting direct access to internal object details (such as variables, methods) from outside.

Data within the class are accessible by functions inside the class, but not by outside functions.

For example, in a banking application, access to confidential data such as account numbers, credentials are restricted from outside.

#### Polymorphism

The term polymorphism comes from the Greek roots _poly_ (many) and _morph_ (form). 

Polymorphism is the ability of an object to have many forms.

**Types of polymorphism**:

* Compile-time/static polymorphism

    Compile-time polymorphism is resolved during the compilation process.
    It is implemented through **method overloading**.

    Method overloading refers to creating multiple methods with the same name but different parameters in the same class.

* Runtime/dynamic polymorphism

    Runtime polymorphism is resolved at runtime. 
    It is implemented through **method overriding**.

    Method overriding allows a subclass to have a different implementation of a method already declared in the superclass.