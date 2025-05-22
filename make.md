make dev



Common Targets:
    build        Build source code and other artifacts for host platform.
    build.all    Build source code and other artifacts for all platforms.
    clean        Remove all files created during the build.
    distclean    Remove all files created during the build including cached tools.
    lint         Run lint and code analysis tools.
    help         Show this help info.
    test         Runs unit tests.
    e2e          Runs end-to-end integration tests.
    generate     Run code generation.
    reviewable   Validate that a PR is ready for review.
    check-diff   Ensure the reviewable target doesn't create a git diff.

Common Options:
    DEBUG        Whether to generate debug symbols. Default is 0.
    PLATFORM     The platform to build.
    SUITE        The test suite to run.
    TESTFILTER   Tests to run in a suite.
    V            Set to 1 enable verbose build. Default is 0.

Release Targets:
    publish      Build and publish final releasable artifacts
    promote      Promote a release to a release channel
    tag          Tag a release

Release Options:
    VERSION      The version information for binaries and releases.
    CHANNEL      Sets the release channel. Can be set to master, main, alpha, beta, or stable.

Go Targets:
    modules.download Download Go modules.
    modules.check    Fail the build if Go modules have changed.
Crossplane Targets:
    submodules            Update the submodules, such as the common build scripts.
    run                   Run crossplane locally, out-of-cluster. Useful for development.


up
---------
up xpkg build
up xpkg push 



crossplane
-------------
crossplane xpkg build
crossplane xpkg push
