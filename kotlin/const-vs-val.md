# Const vs Val

Const are compile time constants, i.e their values are assigned during compiletime, unlike the val where the value is assigned at runtime.

Due to this reason the const cannot be assigned from a function or a constructor.

```kotlin
> const val name = "Aditya" // acceptable

> const val name = getName() // error

> val name = getName() // acceptable
```

Now why const val and not just const ?

Const is not a keyword its just a modifier, just like we use visibility modifiers.

```kotlin
> const val name = "Aditya"

> private val name = "Aditya"
```
