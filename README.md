# Indian Sign Language Translator (ISL)

This project is an **Automatic Indian Sign Language Translator** that converts live spoken English into corresponding Indian Sign Language (ISL) GIFs or alphabet images, providing an assistive tool for the hearing impaired.

## Features

- **Speech Recognition:** Listens to live voice input using your microphone.
- **ISL GIF Display:** Recognizes a wide range of common phrases and displays the matching ISL GIF.
- **Alphabet Spelling:** For unrecognized phrases, spells out each character using ISL alphabet images.
- **Simple GUI:** Uses EasyGUI and Tkinter for user-friendly interaction.
- **Customizable:** Easily extend the list of supported phrases and add new GIFs or alphabet images.

## Demo

![Demo Screenshot](Automatic-Indian-Sign-Language-Translator-ISL/signlang.png)

## Requirements

- Python 3.x
- `speech_recognition`
- `numpy`
- `matplotlib`
- `opencv-python`
- `easygui`
- `Pillow`
- `tkinter` (usually included with Python installations)

Install dependencies using pip:

```bash
pip install speechrecognition numpy matplotlib opencv-python easygui pillow
```

## Usage

1. **Clone the repository**  
   ```
   git clone https://github.com/harsh125op/Indian-sign-language.git
   cd Indian-sign-language
   ```

2. **Prepare assets**  
   - Ensure ISL GIFs are in the folder:  
     ```
     Automatic-Indian-Sign-Language-Translator-ISL/ISL_Gifs/
     ```
   - Ensure alphabet images are in the folder:  
     ```
     Automatic-Indian-Sign-Language-Translator-ISL/letters/
     ```
   - The main GUI image (`signlang.png`) should be in:  
     ```
     Automatic-Indian-Sign-Language-Translator-ISL/
     ```

3. **Run the application**  
   ```
   python isl.py
   ```

4. **How to use:**  
   - The app will show a window with options: "Live Voice" or "All Done!"  
   - Choose "Live Voice" to start speech recognition.
   - Speak a supported phrase (see below) for ISL GIF, or any other phrase to spell it out letter by letter.
   - Say "goodbye", "good bye", or "bye" to exit live voice mode.

## Supported ISL GIF Phrases

The app recognizes dozens of common phrases, such as:

- any questions
- are you angry
- are you busy
- are you hungry
- are you sick
- good morning
- good night
- happy journey
- hello what is your name
- ...and many more!

To see the full list, check the `isl_gif` list in [`isl.py`](isl.py).

## File Structure

```
.
├── isl.py
└── Automatic-Indian-Sign-Language-Translator-ISL
    ├── signlang.png
    ├── ISL_Gifs/
    │   └── <phrase>.gif
    └── letters/
        └── <alphabet>.jpg
```

## Notes

- **Paths:**  
   The script uses absolute paths for images. Update them if your folder structure is different.
- **Adding New Phrases:**  
   Add the phrase (in lowercase) to the `isl_gif` list and place a matching GIF in `ISL_Gifs/`.
- **Alphabet Images:**  
   Place images named `a.jpg`, `b.jpg`,
