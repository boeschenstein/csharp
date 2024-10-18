# C#

## Async/Await

How it really works: <https://devblogs.microsoft.com/dotnet/how-async-await-really-works/>

## Lists

- Collections and Data Structures <https://learn.microsoft.com/en-us/dotnet/standard/collections/>
- Array (fixed size, Range, Indices), Collection, List, Dictionary, Stack, Queue: <https://exceptionnotfound.net/csharp-in-simple-terms-13-arrays-and-collections/>
- ArrayList, Hashtable: <https://azuliadesigns.com/introduction-programmming/collection-types-array-list-dictionary-hash-table/>
- Compare Performance <https://tutorials.eu/c-sharp-collections-performance/>
- Hashtable vs Dictionary vs HashSet <https://www.shekhali.com/csharp-hashtable-vs-dictionary-vs-hashset/>
- Mystery of Equality in C#: IEquatable<T>, IEqualityComparer<T>, IComparable<T>, IComparer<T>: <https://sasan-salem.medium.com/mystery-of-equality-in-c-iequatable-t-iequalitycomparer-t-icomparable-t-icomparer-t-ab98bd2fe541>
  - Record equality: <https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/types/records#value-equality>

## System.IO

<https://devblogs.microsoft.com/dotnet/the-convenience-of-system-io/>

## C# 12

- <https://learn.microsoft.com/en-us/dotnet/csharp/whats-new/csharp-12>
- <https://learn.microsoft.com/en-us/dotnet/csharp/whats-new/tutorials/primary-constructors>

## Exceptions

- Podcast unhandled exception: <https://unhandledexceptionpodcast.com/posts/0072-exceptions/Exceptions>
- <https://learn.microsoft.com/en-us/dotnet/standard/design-guidelines/using-standard-exception-types>
  - ❌ DO NOT throw System.Exception 
  - ❌ DO NOT throw or derive from ApplicationException.
  - ✔️ DO throw an InvalidOperationException if the object is in an inappropriate state.
  - ✔️ DO throw ArgumentException or one of its subtypes if bad arguments are passed to a member. Prefer the most derived exception type, if applicable.
- <https://learn.microsoft.com/en-us/dotnet/standard/design-guidelines/exceptions>
- <https://learn.microsoft.com/en-us/dotnet/standard/exceptions/best-practices-for-exceptions>
  - While it's best to use predefined exception types when possible, you shouldn't raise some reserved exception types, such as AccessViolationException, IndexOutOfRangeException, NullReferenceException and StackOverflowException. For more information, see CA2201: Do not raise reserved exception types.
- Best Practice <https://learn.microsoft.com/en-us/dotnet/standard/exceptions/best-practices-for-exceptions>

## Dispose

- <https://learn.microsoft.com/en-us/dotnet/standard/design-guidelines/dispose-pattern>

## Documentation

- <https://learn.microsoft.com/en-us/dotnet/csharp/tour-of-csharp/>
- dotnet runtime code <https://github.com/dotnet/runtime/tree/main/src/libraries>
- <https://learn.microsoft.com/en-us/dotnet/standard/design-guidelines/>
  - Naming Guidelines: Provides guidelines for naming assemblies, namespaces, types, and members in class libraries.
  - Type Design Guidelines: Provides guidelines for using static and abstract classes, interfaces, enumerations, structures, and other types.
  - Member Design Guidelines: Provides guidelines for designing and using properties, methods, constructors, fields, events, operators, and parameters.
  - Designing for Extensibility: Discusses extensibility mechanisms such as subclassing, using events, virtual members, and callbacks, and explains how to choose the mechanisms that best meet your framework's requirements.
  - Design Guidelines for Exceptions: Describes design guidelines for designing, throwing, and catching exceptions.
  - Usage Guidelines: Describes guidelines for using common types such as arrays, attributes, and collections, supporting serialization, and overloading equality operators.
  - Common Design Patterns: Provides guidelines for choosing and implementing dependency properties and the dispose pattern.
