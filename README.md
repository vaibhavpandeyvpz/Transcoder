The original library is at [natario1/Transcoder](https://github.com/natario1/Transcoder). There was a well-reported issue with EOS on Android 11 here at [https://github.com/natario1/Transcoder/issues/107](https://github.com/natario1/Transcoder/issues/107) which the author has supposedly fixed in [https://github.com/natario1/Transcoder/pull/118](https://github.com/natario1/Transcoder/pull/118) but unfortunately it has now broke the library and it's completely unusable on the latest release.

So here I maintain the older version with the fix suggested by [https://github.com/NiekAkerboom](https://github.com/NiekAkerboom) at [https://github.com/NiekAkerboom/Transcoder/commit/1af92a07e4acd51256761271444899581754e765](https://github.com/NiekAkerboom/Transcoder/commit/1af92a07e4acd51256761271444899581754e765) applied to the last minor version which all works good together.

To use it in your projects, add the [Jitpack]() to your project's root `build.gradle` as shown below:

```groovy
allprojects {
  repositories {
    // ... other repositories e.g., Google, Maven etc. ...
    maven { url 'https://jitpack.io' }
  }
}
```

Then include below dependency in your module's `build.gradle` as follows:

```groovy
dependencies {
  // ... other dependencies ...
  implementation 'com.github.vaibhavpandeyvpz:android-transcoder:0.9.1-android11'
}
```
