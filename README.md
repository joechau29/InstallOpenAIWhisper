## OpenAI Whisper 

## 1. Install Anaconda
1.1 Download it from https://www.anaconda.com/products/distribution.
1.2 Install it.
## 2. Install Git
(a) Download 64-bit Git from https://git-scm.com/download/win
**OR**
(b) run `winget install --id Git.Git -e --source winget` from Command Prompt.
## 3. Install Whisper
3.1 Go to "Anaconda PowerShell Prompt (Anaconda3)".
<img src="https://github.com/joechau29/InstallOpenAIWhisper/blob/main/3.1.png" width=300>
3.2 Install whisper
> (base) PS C:\Users\joechau29> `pip install git+https://github.com/openai/whisper.git`

<img src="https://github.com/joechau29/InstallOpenAIWhisper/blob/main/3.2.png" width=400>

# 4. Install Chocolatey
4.1 Run "Windows PowerShell",  as Administrator.
<img src="https://github.com/joechau29/InstallOpenAIWhisper/blob/main/4.1.png" width=300>
4.2 Install the Chocolatey.

> PS C:\windows\system32>`Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))`

# 5. Install ffmpeg
> (base) PS C:\Users\joechau29> `choco install ffmpeg`