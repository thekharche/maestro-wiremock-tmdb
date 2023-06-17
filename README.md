# Mock with WireMock, UI Test with Maestro

Developing and testing applications that utilize third-party APIs can present a unique set of challenges. These can include dependencies between teams and the unavailability of external APIs during testing phases. These obstacles can slow down the development process and make testing less efficient. One solution to these issues is API mocking, a technique that can expedite development and enhance the flexibility of testing.

## Instruction for Mock

Read at: https://blog.mobile.dev/

## Setup Android App

Open Project in Android Studio.

Create `apikey.properties` in the root directory and add your TMDB API key.

```
NEATFLIX_API_KEY="YOUR_API_KEY"
```

Update your BASE_URL in Constants.kt

```
const val BASE_URL = "YOUR_WIREMOCK_URL_HERE"
```

Run the app.

### Run Maestro UI Test

Download Maestro: https://maestro.mobile.dev/

Run sample UI test
```
maestro test .maestro/flow.yaml
```

## Thanks

For App Code:

https://github.com/Ericgacoki/NeatFlix