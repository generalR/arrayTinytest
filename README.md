jQuery forEach API återskapad baserat på MDN:s beskrivning.

Vad gör forEach?
The forEach() method executes a provided function once per array element.

Syntax
arr.forEach(callback[, thisArg])

Parameter

callback
Function to execute for each element, taking three arguments:

currentValue
The current element being processed in the array.

index
The index of the current element being processed in the array.

array
The array that forEach() is being applied to.

thisArg Optional
Value to use as this(i.e reference Object) when executing callback.


Description
forEach() executes the provided callback once for each element present in the array in ascending order. It is not invoked for index properties that have been deleted or are uninitialized (i.e. on sparse arrays).

callback is invoked with three arguments:
the element value
the element index
the array being traversed

If a thisArg parameter is provided to forEach(), it will be passed to callback when invoked, for use as its this value.  Otherwise, the value undefined will be passed for use as its this value. The this value ultimately observable by callback is determined according to the usual rules for determining the this seen by a function.
