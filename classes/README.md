# classes/

One folder per vulnerability class, created when you write it:

```text
classes/sqli/
  vulnerable.py      # a 10 to 15 line Flask route with the flaw (you write it)
  fixed.py           # the same route, fixed (you write it)
  test_sqli.py       # fails against vulnerable.py, passes against fixed.py (you write it)
```

Suggested folder names: `sqli`, `idor`, `path_traversal`.

Keep each route tiny. If it needs more than about 15 lines, you are testing the framework, not the bug.
