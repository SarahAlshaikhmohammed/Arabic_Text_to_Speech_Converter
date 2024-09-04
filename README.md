
# Arabic Text-to-Speech Converter Using gTTS

This project demonstrates how to convert Arabic text to speech using the Google Text-to-Speech (gTTS) library in Python. The resulting audio is saved as an MP3 file.

## Features

- Converts any Arabic text to speech.
- Outputs the speech as an `.mp3` audio file.
- Uses the `gTTS` (Google Text-to-Speech) library.

## Installation

To use this project, you need to have Python installed along with the `gtts` package. You can install the package using the following command:

```bash
pip install gtts
```

## How to Use

1. Clone or download this repository.
2. Edit the `arabic_text` variable in the code to contain the Arabic text you want to convert to speech.
3. Run the script, and the output will be saved as an `.mp3` file.

### Example:

```python
from gtts import gTTS

def text_to_speech_gtts_arabic(text, filename='output_arabic.mp3'):
    tts = gTTS(text=text, lang='ar', slow=False)
    tts.save(filename)
    print(f"Audio content written to file: {filename}")

arabic_text = "السلام عليكم، أنا ساره آل شيخ محمد متدربة في منصة بيان في برنامج رواد التقنية 24."
text_to_speech_gtts_arabic(arabic_text, filename='output_arabic.mp3')
```

In this example, the text `"السلام عليكم، أنا ساره آل شيخ محمد متدربة في منصة بيان في برنامج رواد التقنية 24."` will be converted to speech and saved as `output_arabic.mp3`.

## License

This project is open-source and available under the MIT License.
