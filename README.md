# tdlib-ios-build

A build-only repo. It holds a single GitHub Actions workflow that compiles
[TDLib](https://github.com/tdlib/td)'s `tdjson` library for iOS using TDLib's
own `example/ios/` scripts, and uploads the resulting
`libtdjson.xcframework` (iOS device + simulator slices) as an artifact.

It is public solely because GitHub-hosted macOS runners are free for public
repositories and billed at 10x minutes for private ones. No application source
lives here — the job checks out `tdlib/td` and builds it.

Run it from the **Actions** tab → *Build libtdjson (iOS)* → *Run workflow*.
