# Voice Recorder Application

This is a web-based **Voice Recorder Application** that allows users to record their voice, save audio files with associated transcripts, and manage their recordings efficiently. The app features an intuitive UI with real-time functionality.

## Features

- **Record Voice:** Start and stop voice recordings easily.
- **Transcript Integration:** Display and associate each recording with a specific transcript.
- **Recording Management:**
  - Retry recording for specific transcripts.
  - Delete all recordings with one click.
  - Download all recordings as a ZIP file.
- **Responsive Design:** Works seamlessly across devices and screen sizes.

## Tech Stack

- **HTML/CSS/JavaScript:** For the frontend interface.
- **MediaRecorder API:** To capture audio.
- **JSZip Library:** For creating downloadable ZIP files.
- **Fetch API:** To load transcripts dynamically from a remote URL.

## How It Works

1. **Load Transcripts:**
   - The application fetches a list of transcripts from a specified URL.
   - Transcripts are displayed one at a time for recording.

2. **Start Recording:**
   - Click the `Start` button to begin recording.
   - A visible recording indicator displays during the recording session.

3. **Stop Recording:**
   - Stop the recording and save the audio file.
   - The recorded audio is linked with the currently displayed transcript.

4. **Manage Recordings:**
   - Retry: Re-record audio for any transcript.
   - Download: Download all recordings as a ZIP file, with a mapping of filenames to transcripts.
   - Delete: Clear all recordings.

5. **Display Recordings:**
   - The app displays all recordings in a table format, including the filename, transcript, and audio player.

## Getting Started

### Prerequisites

Ensure you have a modern web browser that supports the following features:
- MediaRecorder API
- Fetch API
- JavaScript ES6

### Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/anhducmata/voice-recording-for-training.git
    ```

2. Open the `index.html` file in a web browser.

3. Start recording and explore the functionality.

### Live Demo

You can access the live version of the app [here](#).

## File Structure

```
/
└── index.html          # Main HTML file containing all code (HTML, CSS, JavaScript)
```

## Customization

To use your own transcript file:

1. Update the `dataUrl` variable in the script to point to your file:
    ```javascript
    let dataUrl = "https://your-url-to-transcripts.txt";
    ```

2. Ensure the transcript file follows the format:
    ```
    1|First transcript line
    2|Second transcript line
    3|Third transcript line
    ```

## Dependencies

- [JSZip](https://stuk.github.io/jszip/) for handling ZIP file creation.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to improve the app.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Happy recording!
