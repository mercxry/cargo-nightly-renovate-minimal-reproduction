# Current behaviour

Renovate bot creates the PRs for the outdated crates, but is unable to parse the `Cargo.toml` file because it is using a nightly feature `workspace-inheritance`, while the renovate bot is on the stable channel.

# Expected behaviour

Renovate bot should check if the root directory has a `rust-tooolchain.toml` or a `rust-tooolchain` file and use it to install the correct rust channel for the project.
