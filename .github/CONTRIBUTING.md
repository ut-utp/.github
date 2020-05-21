## Contributing to the `ut-utp` repos

Thanks for considering contributing! Here are some of the conventions we try to follow in our repos.

### Commit names

This is very optional, but we (mostly) start our commit messages with a tag indicating what part of the repo the commit actually touches. For example, [`sim: reorder reset`](https://github.com/ut-utp/core/commit/2a893a981b9dc66d751b1f3bc217e78b39c39ed9).

This makes it easier to tell what parts of the project end up getting worked on more. There isn't a formal list of tags that are used in a repo, and it's all very ad-hoc (though, at least for [core](https://github.com/ut-utp/core) they mostly match the crates).

Actually using the tags isn't required but is encouraged. Feel free to introduce new tags when appropriate.
Here's a one-liner to see what tags are used:
    ```bash
    alias git-log-stat='git log --oneline | cut -d ' ' -f2- | grep '^[^ ]*:.*$' | cut -d ':' -f 1 | sort | uniq -c | sort -hr'
    ```

### Formatting

All of our Rust repos _should_ run `rustfmt` in CI. Regardless, we encourage you to run `cargo fmt` locally before submitting a PR.

### Linking to issues

A lot of the TODOs in the codebase try to point back to the issue that tracks them by mentioning the issue number they correspond to:
```rust
// TODO(#12): add a doc test that shows the foo-bar with the baz causing a compile error
```

This is very optional; just having the links go one way (i.e. having permalinks to relevant code blocks) is usually good enough.

### Licensing

Unless you say otherwise, all contributions submitted will be licensed as per the LICENSE file of the repo you're contribution was made to.
