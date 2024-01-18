# Unreleased

# 0.2.0

**Breaking Changes**

- Rework crate into a middleware

This changes the structure of the crate such that it is now a middleware in addition to being an extractor. Doing so allows us to improve the ergonomics of the API such that calling `save` and awaiting a future is no longer needed.

Now applications will need to install the `MeessagesManagerLayer` after `tower-sessions` has been installed (either directly or via a middleware that wraps it).

Also note that the iterator impplementation has been updated to use `Message` directly. Fields of `Message` have been made public as well.

# 0.1.0

- Initial release :tada: