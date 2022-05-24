# qscanr
## QR and BARCODE scanner using kivymd

Convert this to apk using following steps and use in you android phone:
#### Step-1:
Clone this repo using `git clone https://github.com/saurabh190802/qscanr.git`
#### step-2:
Open a new notebook in Google Colab. [link](https://colab.research.google.com/)
#### step-3:
uplod main.py folder to colab.
#### step-4:
run all this commands in colab one by one.
`!pip install buildozer`<br>
`!pip install cython==0.29.19`<br>
`!sudo apt-get install -y \
    python3-pip \
    build-essential \
    git \
    python3 \
    python3-dev \
    ffmpeg \
    libsdl2-dev \
    libsdl2-image-dev \
    libsdl2-mixer-dev \
    libsdl2-ttf-dev \
    libportmidi-dev \
    libswscale-dev \
    libavformat-dev \
    libavcodec-dev \
    zlib1g-dev`<br>
`!sudo apt-get install -y \
    libgstreamer1.0 \
    gstreamer1.0-plugins-base \
    gstreamer1.0-plugins-good`<br>
`!sudo apt-get install build-essential libsqlite3-dev sqlite3 bzip2 libbz2-dev zlib1g-dev libssl-dev openssl libgdbm-dev libgdbm-compat-dev liblzma-dev libreadline-dev libncursesw5-dev libffi-dev uuid-dev libffi6`<br>`!sudo apt-get install libffi-dev`<br>
`!buildozer init`<br>
This will generate an buildozer.spec file edit the requirement section there add kivymd and pillow to it.
change others if required.<br>
`!buildozer -v android debug`<br>
After this an apk file will be generated there inside bin file.<br>
Download that take to your android phone and use....<br>
`!buildozer android clean`
