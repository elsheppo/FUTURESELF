# FutureSelf

FutureSelf is an innovative personal motivation tool that uses AI to transform your to-do list into encouraging voice messages from your "future self". Built entirely with iOS Shortcuts, it combines the power of local language models, voice cloning, and automated messaging to keep you motivated and on track.

## Features

- Pulls task lists from Apple Reminders (can be shared with other users as well)
- Generates motivational messages using a local LLM (Ollama, llama3)
- Converts text to speech using your own cloned voice (ElevenLabs)
- Sends audio messages to your phone

## Prerequisites

- Apple devices with Shortcuts app installed
- Mac with Ollama installed (https://ollama.ai)
- ElevenLabs account with a cloned voice (https://elevenlabs.io)
- (Optional) Pushcut app for automated running of shortcuts (https://www.pushcut.io)

## Setup

1. Install Ollama on your Mac and ensure it's running.
2. Clone your voice using ElevenLabs and note your API key and voice ID.
3. Create a new shortcut in the Apple Shortcuts app.
4. Set up the following actions in your shortcut:
   - Get reminders from a specific list
   - Run a shell script over SSH to call Ollama on your Mac
   - Call ElevenLabs API to generate speech from text
   - Send a message to yourself with the audio file

## Usage

1. Run the shortcut manually whenever you want a motivational boost.
2. (Optional) Set up automated running:
   - Use the Shortcuts app to schedule regular runs
   - Or use Pushcut for more advanced automation options

## Configuration

- Customize the prompt used for the LLM to match your preferred motivational style.
- Adjust the frequency of messages to suit your needs.
- Experiment with different voice clones or styles in ElevenLabs.

## Privacy and Security

- All processing is done locally on your devices or through your personal ElevenLabs account.
- No data is stored or processed by third-party servers (except for the ElevenLabs API call).

## Troubleshooting

- Check that Ollama is running on your Mac before executing the shortcut.
- Verify your ElevenLabs API key and voice ID are correct.

## Future Enhancements

- Integrate with more task management apps
- Add support for multiple users (coach/student model)
- Implement mood detection to tailor motivation style

## Acknowledgments

- Ollama team for their amazing local LLM tech
- ElevenLabs for their voice cloning technology
- Apple for the powerful Shortcuts app

---

Remember: Stay motivated, your future self believes in you!
