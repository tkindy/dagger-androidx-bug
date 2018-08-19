# dagger-androidx-bug

Minimal repro for [google/dagger#1245](https://github.com/google/dagger/issues/1245)

### Steps to Reproduce

1. Checkout `androidx` branch
1. `./gradlew clean assembleDebug`

### Notes

- `master` builds fine. It appears switching to `androidx` dependencies (even with Jettifier enabled) causes Dagger to fail to process the repo.
- switching to Dagger 2.16 on the `androidx` branch allows it to build fine
