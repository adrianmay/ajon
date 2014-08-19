ajon
====

_More Accurate Than JSON_

It may be a problem for some projects (including rhaboo) that JSON mangles arrays: non-numerically named properties are discarded and nulls are filled into all the sparse positions (wheras JS objects in memory can distinguish between property values of null, undefined and deleted.)

This module provides stringify(object) and parse(string) analogous to JSON such that arrays are preserved properly.

There's no attempt to deal with prototypes or function-valued properties. Regexes are not dealt with yet but could be.

The serialised notation is not pretty enough to read for pleasure, and there are no customisation options. It's only intended for computers to read.
