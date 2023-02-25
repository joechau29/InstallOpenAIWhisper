## Install OpenAI Whisper in Virtual Environment

### 1. Install Anaconda
1.1 Download it from https://www.anaconda.com/products/distribution.
1.2 Install it.

### 2 Install Git
2.1 Download 64-bit Git from https://git-scm.com/download/win
2.2 Install it.

### 3. Install Chocolatey
3.1 Run "Windows PowerShell",  as Administrator.

<img src="https://github.com/joechau29/InstallOpenAIWhisper/blob/main/3.1.png" width=300>

3.2 Install the Chocolatey.

> **PS C:\windows\system32>**`Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))`

### 4. Install ffmpeg
4.1 Run "Windows PowerShell",  as Administrator.
4.2 Install ffmpeg.
> PS C:\windows\system32> `choco install ffmpeg`

4.3 Type `Y` and  press `Enter` for " "Do you want to run the script?"

### 5. Creating virtual environment
5.1 Run "Anaconda PowerShell".
5.1 Execute `python -m venv C:\Users\frog\venv` to create the virtual environment.
5.2 Execute `C\Users\frog\venv\activate.bat` to activate the virtual environment.  The prompt will be changed as below: -
> **(venv)** (base) C:\Users\frog>

### 6. Install Whisper
6.1 Run "Anaconda PowerShell".

<img src="https://github.com/joechau29/InstallOpenAIWhisper/blob/main/6.1.png" width=300>
6.2 Install whisper
>**(venv)** (base) PS C:\Users\frog> `pip install git+https://github.com/openai/whisper.git`

<img src="https://github.com/joechau29/InstallOpenAIWhisper/blob/main/6.2.png" width=400>

## Run Open AI Whisper
1.1 Activate virtual environment.  **Anaconda PowerShell** `C\Users\frog\venv\activate.bat`
1.2 Execute `whisper [source file] --model [tiny/base/small/medium/large][.en]`

*Notes* : model sizes: larger the size, much accurate with lower converting speed.

Examples:
Convert a mp4 and the content is understanable Enlgish
 `whisper c:\Users\frog\gorilla_speak_understandable_english.mp4 --model tiny.en`
Convert a mp4 and the content is in multi-languages
`whisper c:\Users\frog\gorilla_speak_chinglish.mp4 --model tiny`
Convert a mp4 in Cantonese with assent
`whisper c:\Users\frog\gorilla_speak_chinglish.mp4 --model small`

References: 
1. https://github.com/openai/whisper/blob/main/README.md
2. https://www.youtube.com/watch?v=HSVjz4FPKzM