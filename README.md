## OpenAI Whisper 

## 1. Install Anaconda
1.1 Download it from https://www.anaconda.com/products/distribution.
1.2 Install it.
## 2. Install Git
2.1 Download 64-bit Git from https://git-scm.com/download/win
## 3. Install Whisper
3.1 Go to "Anaconda PowerShell Prompt (Anaconda3)".

<img src="https://github.com/joechau29/InstallOpenAIWhisper/blob/main/1.png" width=300>
3.2 Install whisper

> (base) PS C:\Users\joechau29> `pip install git+https://github.com/openai/whisper.git`

<img src="https://github.com/joechau29/InstallOpenAIWhisper/blob/main/2.png" width=400>

# 4. Install Chocolatey
In "Anaconda PowerShell Prompt (Anaconda3)",  install the Chocolatey.

> (base) PS C:\Users\joechau29> `Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))`

# 5. Install ffmpeg
> (base) PS C:\Users\joechau29> `choco install ffmpeg`
