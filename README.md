# Installing packages from `apt` repositories

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/binder-examples/apt_install/master?filepath=index.ipynb)

Sometimes you want packages that exist outside of the language-specific packaging
ecosystems of Python/R/Julia. Binder makes it possible to `apt-install` packages
from the ubuntu apt repository. This repository demonstrates how to do this by specifying
names in an `apt.txt` file.

## Notes
The `apt.txt` file should list all packages that your notebooks
depend on, and they will be installed using:

```
apt-get install --yes --no-install-recommends
```

The base Binder image contains no extra dependencies, so be as
explicit as possible in defining the packages that you need.

In this example we include the tools `cowsay` and `lolcat` which will be installed in
the environment, and our notebook uses them to show a colorful message.
