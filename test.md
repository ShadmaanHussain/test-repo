Tests to see how GitHub and GitLab work exactly and to detect bugs with them.

Tests that are very large will not be included here to keep this repository small:

- <https://github.com/cirosantilli/test-deep>
- <https://github.com/cirosantilli/test-diff-many-files>
- <https://github.com/cirosantilli/test-pr-many-commits>

There are also some tests that could not be included here conveniently:

- <https://github.com/cirosantilli/test-empty-commit>
- <https://github.com/cirosantilli/test-empty-subdir>
- <https://github.com/cirosantilli/test-long-filename>

This repository is mirrored at:

- <https://github.com/cirosantilli/test>
- <https://gitlab.com/cirosantilli/test>

Other similar repos from other people:

- <https://github.com/joernchen/evil_stuff>

The most interesting files on this repository are:

-   [markdown.md](markdown.md)

-   whitespace filename edge cases:

    - [single whitespace filename](%20)
    - [double whitespace directory name](%20%20/) and [it's README](%20%20/README.md)
    - [a b](a b)

Some interesting branches include:

-   [`hasslash/a`](../hasslash/a): branch inside sub-directory

-   [`-r`](../-r): branch with forbidden name, and in particular one that may be used for shell injection. 

    Create manually with `cp master -- -r` and push with `git push --all`.