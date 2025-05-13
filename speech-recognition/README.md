# WEB SPEECH API

[Reference Link](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API)

## How to run this?
`tsc -d -p ./tsconfig.json` (makes use of config from tsconfig.json)
  
`tsc -d index.ts` (goes with default config)

Run any of the above commands in Command prompt to compile ts files to js files and open index.html in browser

## Steps followed in code

- Create UI components
- create SpeechRecognition Object
- create grammar using ([JSGF - JSpeech Grammar Format](https://www.w3.org/TR/jsgf/))
- Attach grammar to SpeechRecognition object and configure other variables (continuous, interimResults, lang, maxAlternatives)
- Based on any user event, trigger start function from SpeechRecognition object created to start listening
- Get the result in onresult callback of SpeechRecognition object created
- Process it (optionally) and display to User or feed to any AI Model for processing
