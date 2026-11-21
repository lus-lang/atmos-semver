# semver

Parses, compares, and matches semantic versions with the range syntax of npm.

```lus nocheck
local semver = require("https://atmosp.here/2.0/semver.lus")

print(semver.satisfies("1.4.2", "^1.2"))                       --> true
print(semver.max_satisfying({ "1.2.0", "1.9.1", "2.0.0" }, "~1.9"))   --> 1.9.1
```

The package requires Lus 2.0. It declares no permissions. It calls no `pledge` of its own, so the program that loads it keeps control of its permissions.

The reference is in the doc comments of `semver.lus`. Run `lus doc semver.lus` to print it.
