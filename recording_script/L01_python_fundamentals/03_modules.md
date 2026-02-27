So far we've been working with Python's built-in capabilities -- basic arithmetic, strings, booleans. But the real power of Python for data work comes from something else entirely: its ecosystem of packages.

Python is designed to be intentionally lightweight at its core. Rather than trying to do everything out of the box, Python allows specialists to build packages -- self-contained bundles of code -- that extend what Python can do. The pandas team focuses exclusively on building the best possible tools for data manipulation. The matplotlib team focuses on visualization. Because each team can focus deeply on their domain, you end up with best-in-class tools for each task rather than a single language trying to do everything adequately.

As economists, a handful of packages will become our bread and butter. We'll use `pandas` for loading, cleaning, and reshaping data. We'll use `numpy` for numerical computing. We'll use `matplotlib` for visualization. We're not ready to dig into those just yet, but understanding how packages work is a foundational skill that everything else will depend on.

To use a package, we write `import package` at the top of our notebook. After that, we access anything inside the package using dot notation: `package.thing_we_want`. This is the same dot notation you saw when we used string methods -- the dot is Python's way of saying "look inside this object."

<Talk about importing a package>

* Use `import sys` as a simple first example
* Show `sys.version` to illustrate dot notation -- we're reaching inside the `sys` package to grab the `version` information
* Point out that `import` statements are typically placed at the top of a notebook so it's clear what the notebook depends on

<Talk about package aliases>

* Some package names are long and it would be tedious to type them in full every time -- Python lets us give a package a shorter nickname using `import package as alias`
* Show `import pandas as pd` and demonstrate calling `pd.DataFrame.from_dict(...)` -- give students a preview of what pandas can do without getting into the details
* Emphasize that while you can choose any alias, there are strong conventions: `pd` for pandas, `np` for numpy, `mpl` for matplotlib, `dt` for datetime
* Two reasons to stick to conventions: your code is immediately readable to other Python users, and coding tools like AI assistants will use the same conventions

<Talk about the math package>

* Use `import math` as a hands-on example for students to explore
* Demonstrate tab completion on `math.` to browse what's available inside the package
* Good opportunity for students to practice finding and using things they haven't been explicitly taught -- a skill they'll need throughout the course
