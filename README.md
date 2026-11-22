# semver

`semver` parses, compares, and matches semantic versions with the range syntax of npm.

The following example checks which versions of a dependency a range accepts.

```lus nocheck
local semver = require("https://atmosp.here/2.0/semver.lus")

print(semver.satisfies("1.4.2", "^1.2"))                       --> true
print(semver.max_satisfying({ "1.2.0", "1.9.1", "2.0.0" }, "~1.9"))   --> 1.9.1
```

The package requires Lus 2.0 and declares no permissions. It never calls `pledge`, so the program that loads it keeps control of its permissions.

The reference is in the doc comments of `semver.lus`, which `lus doc semver.lus` prints.
