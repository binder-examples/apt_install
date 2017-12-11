# Installing packages from apt with `apt.txt`

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/binder-examples/apt_install/master?filepath=index.ipynb)

Sometimes you want packages that exist outside of the language-specific packaging
ecosystems of Python/R/Julia. `repo2docker` makes it possible to apt-install packages
from the ubuntu apt repository. This repository demonstrates how to do this by specifying
names in an `apt.txt` file.