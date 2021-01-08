# bazel-build-android

## setup
```
git clone https://ranaaditya/bazel-build-android
```
## build
```
npm install -g @bazel/bazelisk
cd bazel-build-android
bazel build //app//src/main:app
```

## deploying on device
connect your android device to adb


```
bazel build //app/src/main:app mobile-install
```

### to start the app on deployment

```
bazel build //app/src/main:app mobile-install --start_app
```

## clean build

```
bazel clean
bazel build //app//src/main:app
```