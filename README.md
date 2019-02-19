[![Build Status](https://dev.azure.com/stefurishin/SparseNumerics/_apis/build/status/SparseNumerics-CI?branchName=master)](https://dev.azure.com/stefurishin/SparseNumerics/_build/latest?definitionId=2&branchName=master) [![Nuget Package](https://img.shields.io/nuget/v/SparseNumerics.svg)](https://www.nuget.org/packages/SparseNumerics/)



## `SparseNumerics.SparseInteger`

A value of this type represents a non-negative integer that can be very large (like those that occur as
numeric values of high power towers, much larger than those that can be represented by `BigInteger`
within feasible memory limits), subject to a condition that either:

- the number fits into `ulong` type verbatim

- the number of 1's in its binary form is a moderate number (such that an array of that size can be allocated), and each of the positions of 1's in its binary form is, recursively, a number that can be represented by `SparseInteger`.

Code originally taken from https://github.com/VladimirReshetnikov/Oeis.A002845
