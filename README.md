# C#

## .NET

- .NET <https://github.com/boeschenstein/dotnet/blob/main/README.md>
- C# = Language, .NET = Runtime <https://www.linkedin.com/pulse/understanding-difference-between-net-c-enfixo>

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

### Helpers

```
ArgumentNullException.ThrowIfNull
ArgumentException.ThrowIfNullOrEmpty(String, String)
ArgumentException.ThrowIfNullOrWhiteSpace(String, String)
ArgumentOutOfRangeException.ThrowIfZero<T>(T, String)
ArgumentOutOfRangeException.ThrowIfNegative<T>(T, String)
ArgumentOutOfRangeException.ThrowIfEqual<T>(T, T, String)
ArgumentOutOfRangeException.ThrowIfLessThan<T>(T, T, String)
ArgumentOutOfRangeException.ThrowIfNotEqual<T>(T, T, String)
ArgumentOutOfRangeException.ThrowIfNegativeOrZero<T>(T, String)
ArgumentOutOfRangeException.ThrowIfGreaterThan<T>(T, T, String)
ArgumentOutOfRangeException.ThrowIfLessThanOrEqual<T>(T, T, String)
ArgumentOutOfRangeException.ThrowIfGreaterThanOrEqual<T>(T, T, String)
ObjectDisposedException.ThrowIf 
```

## Dispose

- <https://learn.microsoft.com/en-us/dotnet/standard/design-guidelines/dispose-pattern>

## Documentation

- <https://learn.microsoft.com/en-us/dotnet/csharp/tour-of-csharp/>
