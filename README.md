[![Status](https://img.shields.io/badge/status-active-success.svg?style=flat-square&logo=flutter)](https://github.com/rydam1403/Drishti)
[![made-with-flutter](https://img.shields.io/badge/made%20with-flutter-blue.svg?style=for-the-badge&labelColor=03045e&logo=flutter)](https://flutter.dev)
[![forthebadge](https://forthebadge.com/images/badges/built-by-developers.svg)](https://forthebadge.com)

<br />
<div align="center">
  <a href="https://github.com/rydam1403/Drishti">
    <img src="assets/eye.png" alt="Logo" width="120" height="120" align="center">
  </a>

  <h2 align="center">Drishti</h2>

  <p align="center">
    A Flutter app for blind people.
    <br />
    <br />
    <a href="https://github.com/rydam1403/Drishti/issues">Report Bug</a>
    ·
    <a href="https://github.com/rydam1403/Drishti/issues">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [Table of Contents](#table-of-contents)
- [About The Project](#about-the-project)
  - [Built With](#built-with)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Thank You!](#thank-you)
- [Acknowledgements](#acknowledgements)

<!-- ABOUT THE PROJECT -->

## About The Project

|                            Face Recognition                             |                            Object Detection                             |                      OCR with speech output                      |                            Text Summarization                            |                               Google Translate API                               |
| :---------------------------------------------------------------------: | :---------------------------------------------------------------------: | :--------------------------------------------------------------: | :----------------------------------------------------------------------: | :------------------------------------------------------------------------------: |
| <img src="images/recognizeface.gif" alt="Recognize Face" height="300"/> | <img src="images/objectdetect.gif" alt="Detect Objects" height="300" /> | <img src="images/ocrdoing.gif" alt="OCR for text" height="300"/> | <img src="images/summarizetext.gif" alt="Summarize Text" height="300" /> | <img src="images/googletranslate.gif" alt="Google Translate API" height="300" /> |

|                                 GPS Location Tracing                                  |                                Video Call Backend Server                                |                             Video Call App Client                             |
| :-----------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------: |
| <img src="images/locationtracer.png" alt="Trace Location" height="300" width="400" /> | <img src="images/videobackend.jpg" alt="Video Call Backend" height="300" width="400" /> | <img src="images/videofrontend.jpg" alt="Video Call Frontend" height="300" /> |

> Please wait for sometime for the above GIFs to load. Otherwise, click on them to view them individually.

This is a Flutter app that uses [Firebase ML vision](https://firebase.google.com/docs/ml), [Tensorflow Lite](https://www.tensorflow.org/lite), and in-built speech recognition and text-to-speech capabilities to act like a third eye for blind people. It uses Firebase ML vision to detect human faces, and Tensorflow Lite model implementations of [MobileFaceNets](https://arxiv.org/abs/1804.07573) and [SSD MobileNetV2](https://arxiv.org/abs/1801.04381) to perform face recognition and object detection respectively. The blind user can authenticate with fingerprint, issue voice commands to perform face recognition, object detection, OCR, automatic URL and text summarization, translate languages, send GPS location, and perform video calling with volunteer. The app responds appropriately via voice output for every command issued. The text summarization API is built with Flask, Sumy, Trafilatura and is deployed to Heroku. It uses Latent Semantic Analysis(LSA) algorithm for text summarization. The blind user can use this app to detect and save human faces, detect objects in front of him/her, get voice output of text within objects, summarized result of text and URLs, translate sentences to different languages, video call, and also send his/her GPS location for tracing purposes.

### Built With

This project is entirely built with the following components and languages:

- [Flutter](https://flutter.dev/)
- [Firebase ML vision](https://firebase.google.com/docs/ml)
- [Google Translate API](https://cloud.google.com/translate)
- [Tensorflow Lite](https://www.tensorflow.org/lite)
- [MobileFaceNets](https://arxiv.org/abs/1804.07573)
- [SSD MobileNetV2](https://arxiv.org/abs/1801.04381)

<!-- GETTING STARTED -->

## Getting Started

You can download the pre-built apk file found in the `Releases` section. Follow these instructions in order to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Java Runtime Environment(JRE)>=8, Android SDK API level 28 or higher should be installed. Flutter and Dart SDKs should be installed. After installation, check Java version, and Flutter configuration using

```sh
java --version
flutter doctor
```

### Installation

1. Download or Clone the repo

```git
git clone https://github.com.git/rydam1403/Drishti.git
```

2. Open the downloaded project folder

```sh
cd Drishti
```

3. Make sure Flutter executable is added to environment variables. Go to project root and execute the following command in console to get the required dependencies

```sh
flutter pub get
```

4. Connect your Android device to your desktop. Make sure it is properly connected by using

```sh
flutter devices
```

5. Install and run the app using

```sh
flutter run
```

<!-- USAGE EXAMPLES -->

## Usage

Once the app starts, authenticate yourself with fingerprint. Then, tap to issue voice commands like `recognize face`, `detect objects`, `read text` and `send my location` to perform respective functionalities. In face recognition screen, double tap to change camera, and once human face is detected, long tap to save detected face. The name for detected face can be given with voice input by tapping onto screen.



<!-- LICENSE -->

## License

Distributed under the MIT License.

## Thank You!

[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)

If you like this project, please ⭐ this repo and share it with others 👍

<!-- ACKNOWLEDGEMENTS -->

## Acknowledgements

- [Flutter Docs](https://flutter.dev/docs)
- [Firebase ML Docs](https://firebase.google.com/docs)
- [Tensorflow Lite Docs](https://www.tensorflow.org/lite/guide)
- [MobileFaceNets](https://arxiv.org/abs/1804.07573)
- [SSD MobileNetV2](https://arxiv.org/abs/1801.04381)
