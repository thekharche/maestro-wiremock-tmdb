# Mock with Mockoon, UI Test with Maestro

Designing, building, and testing applications consuming third-party APIs can be quite challenging. As developers, we often face bottlenecks such as inter-team dependencies and external API unavailability during testing. API mocking is a solution that helps us overcome these challenges, speeding up development, and making testing more flexible. In this blog post, we will demonstrate how to optimize your UI testing using mock APIs with Mockoon and Maestro.

Read the blog at https://blog.mobile.dev/

## Getting Started

### Mockoon Mock http server

```
npm install -g @mockoon/cli
```

```
mockoon-cli start -d ~/mock-tmdb.json -p 3001
```

### Setup Android App

Open Project in Android Studio.

Create `apikey.properties` in the root directory and add your TMDB API key.

```
NEATFLIX_API_KEY="YOUR_API_KEY"
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