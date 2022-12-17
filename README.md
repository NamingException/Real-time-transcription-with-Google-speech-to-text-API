# Node.js and React Speech-to-Text Demo

This is a simple app that demonstrates how to use the Google Speech-to-Text API in a Node.js and React application.

## Requirements

- Node.js (tested with version 12.x)
- React (tested with version 16.x)
- Google Cloud Platform Credentials with Speech-to-text api permissions
  > Follow this [tutorial](https://console.cloud.google.com/projectselector2/speech/overview?tutorial=speech-to-text__speech-to-text-nodejs&supportedpurview=project) to create credentials and learn how to use the google-speech-to-text API

## Setup

1.  Clone this repository: `git clone https://github.com/untilhamza/Google-speech-to-text-App-in-react.git`

### Frontend part

1.  Navigate to the react-app project directory: `cd stt-client`
2.  Install dependencies: `yarn`
3.  Start the development server: `yarn start`
4.  Navigate back to the parent directory : `cd..`

The app will now be running at [http://localhost:3000](http://localhost:3000/).

### Add Credentials

1. Make sure to get google cloud credentials as shown in this [tutorial](https://console.cloud.google.com/projectselector2/speech/overview?tutorial=speech-to-text__speech-to-text-nodejs&supportedpurview=project)
2. Copy the generated credentials speech-to-text-key.json file save it to the server folder as `speech-to-text-key.json`.
   > This file name is already added to the .gitignore file but make sure not to push to github or any public repositories
3. Navigate to the server folder in the terminal and run this to add google credentials to our node js backend.

```
$ export GOOGLE_APPLICATION_CREDENTIALS="./speech-to-text-key.json"
```

### Backend part

1.  Navigate to the server project directory: `cd server`
2.  Install dependencies: `yarn`
3.  Start the development server: `yarn run dev`
4.  Start the development server: `npm start`

The backend listens at [http://localhost:8081](http://localhost:8081/).

## Usage

To use the app, simply click the "Start Recording" button and speak into your microphone. The transcription will appear on the screen as you speak, updating in real-time. When you're finished, click the "Stop Recording" button to see the final transcription.

## Credits

This app was built by [Hamza](https://github.com/untilhamza) using the Google Speech-to-Text API.

## License

This project is licensed under the MIT License. See the [LICENSE](https://opensource.org/licenses/MIT) file for more details.