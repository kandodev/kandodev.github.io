# Effective Modern C++

Skipping Chapter 1 - Deducing Types (notes in notebook)

## Item 5: Prefer auto to explicit type declarations
* Can directly hold closures. The only replacement is an std::function but that's just using template magic and doesn't actually hold the closure.
* E.g in the cases where it replaces an std::function, i.e. holding a closure, it's even more efficient because there's no need to initialize the std::function template.
* It's also faster to invoke a closure with an auto-declared object.
* 

## Item 6: ...
--
## Item 7: Distinguish between () and {} when creating objects
* Three types of initializations:
  * int x = 2;
  * int x(2);
  * int x { 2 };
* Braced/Uniform initialization uses {}. Is an attempt to have an intiialization syntax that can be used everywhere.
* Also prohibits implicit narrowing conversions among built-in types. In other initalizations, there may be implicit type conversions to make things match.
* Drawback - tangled with std::initializer_lists and ctor overload resolution. In fact, initializer lists match strongly with it even if the types are not exact.
