# Javadoc Conventions

## `@author` Tags

The primary maintainer of the class/interface should be the first `@author` listed. Then other contributors follow, in order of signifigance.

## `@version` Tag

Version tags should follow the SCCS convention, which is as follows:

`@version <major>.<minor> (<latest author>), <month>/<day>/<year>`

- `<major>` is the big version number, this should only be incremented if a large amount of changes are made or the underlying purpose or function of the class changes.
- `<minor>` is the incremental version number, it should always be two digits long (if you get to 99, roll over and increment `<major>`) (also, for 0 or single digit numbers it would be 00, 01, 02, etc.) and should be incemented every change that is made.
- `<latest author>` is the last person to make a change.
- `<month>`, `<day>`, and `<year>` are the date of the last changes. Each number should be two digits long. (e.g. 02/04/02, 12/12/16, etc.)

Here is an example of the tag Zach would change it to, after making a change on version 1.00 on December 19, 2016:

`@version 1.01 (Zach), 12/19/16`

## `@see` Tags

The `@see` tag is used to reference other packages, classes, interfaces, enumerations, fields, contructors, or methods in your doc comment.

Here is a list of all possible `@see` tags and the order they should be arranged in:

1. `@see #field`
2. `@see #Constructor(Type, Type...)`
3. `@see #Constructor(Type id, Type id...)`
4. `@see #method(Type, Type,...)`
5. `@see #method(Type id, Type, id...)`
6. `@see Class`
7. `@see Class#field`
8. `@see Class#Constructor(Type, Type...)`
9. `@see Class#Constructor(Type id, Type id)`
10. `@see Class#method(Type, Type,...)`
11. `@see Class#method(Type id, Type id,...)`
12. `@see package.Class`
13. `@see package.Class#field`
14. `@see package.Class#Constructor(Type, Type...)`
15. `@see package.Class#Constructor(Type id, Type id)`
16. `@see package.Class#method(Type, Type,...)`
17. `@see package.Class#method(Type id, Type, id)`
18. `@see package`
