# Text-to-Speech Automation with Background Music Overlay

## Overview

This project automates the process of converting text data into speech using Google Cloud's Text-to-Speech API and overlays the generated speech with background music using the `pydub` library. The final output is a collection of MP3 files enriched with background audio, suitable for applications like podcasts, audiobooks, or multimedia presentations.

## Prerequisites

Before running the scripts, ensure you have the following installed:

- **Python 3.x**: The programming language used for scripting.
- **Google Cloud Account**: To access the Text-to-Speech API.
- **FFmpeg**: A multimedia framework required by `pydub` for audio processing.
- **Python Libraries**:
  - `pandas`: For handling Excel files.
  - `pydub`: For audio manipulation.
  - `google-cloud-texttospeech`: For interfacing with Google's Text-to-Speech API.

## Setup Instructions

### 1. Just select one Google Cloud Setup, gTTS, ElevenLabs

a.1 **Create a Google Cloud Project**:
   - Navigate to the [Google Cloud Console](https://console.cloud.google.com/).
   - Click on **"Select a Project"** and then **"New Project"**.
   - Provide a name and create the project.

a.2 **Create an account in ElevenLabs**:
   - Get an API to your account.

a.3 **gTTS works without account it is FREE**:

b. **Enable the Text-to-Speech API**:
   - Within your project, go to **"APIs & Services" > "Library"**.
   - Search for **"Text-to-Speech API"** and click **"Enable"**.

c. **Set Up Authentication**:
   - Go to **"APIs & Services" > "Credentials"**.
   - Click **"Create Credentials"** and select **"Service Account"**.
   - Fill in the required details and proceed.
   - After creating the service account, navigate to it and create a **JSON key**.
   - Download the JSON key file and save it securely; you'll need its path later.

### 2. Install FFmpeg

**For Windows**:
- Download the FFmpeg executable from the [official website](https://github.com/BtbN/FFmpeg-Builds/releases).
- select and download ffmpeg-master-latest-win64-gpl file
- Extract the contents and add the `bin` directory to your system's PATH environment variable.
