# Unearthed

A library for Android that notifies you when your app was restored after a
process death.

## Usage

Wherever convenient, add a listener to `Unearthed` and get notified of
restoration after process death.

```kotlin
Unearthed.onProcessRestored { graveyard ->
  Log.d("MainActivity", "App has been restored ${graveyard.gravestones.size}
  times.")
}
```

## Download

Find artifacts on [Maven
Central](https://search.maven.org/search?q=de.hannesstruss.unearthed)
at `de.hannesstruss.unearthed:unearthed:0.1.0`.

## Releasing

    ./gradlew :library:publishMavenAarPublicationToMavenRepository


# License

    Copyright 2020 Hannes Struss
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
       http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
