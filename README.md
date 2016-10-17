# AdvancedOCR

## About:
The **AdvancedOCR** app uses a library for OCR called tess-two(A fork of Tesseract Tools for Android (tesseract-android-tools) that adds some additional functions).

## Pre-requisites
- Android 2.3 or higher
- A v3.02+ trained data file for a language. Data files must be extracted to the Android device in a subdirectory named tessdata.
  
## Usage
To use tess-two from your app, edit your app module's build.gradle file to add tess-two as an external dependency:
```
dependencies {
    compile 'com.rmtheis:tess-two:6.0.4'
}
```

## Assets
Create a folder in your Source directory called `assets`. Inside assets add a new folder called `tessdata` and move the trained data for language file inside this folder.
Therefore the location of the traineddata file will be:
  `\src\main\assets\tessdata\end.traineddata`
  
## Implementation
1. The app provides the user to be able to click a new pic or use a existing image from gallery.
2. Once the pic is clicked or choosen the user is allowed to crop the image and the cropped image is fed to the tesseract to perform OCR and return a string of text.
3. The Text is displayed in the Edit box and the cropped image to shown to the user.

## Support
- [Stack Overflow](https://stackoverflow.com/questions/tagged/tess-two)
- [tesseract-ocr](https://groups.google.com/forum/#!forum/tesseract-ocr)
