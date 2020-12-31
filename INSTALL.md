# AWS Streamer - System Packages Installation

## Ubuntu

- Install Python dependencies:
    ```
    sudo python3 -m easy_install install pip
    sudo python3 -m easy_install install virtualenv
    ```

- Install OS packages:
    ```
    sudo apt-get update
    sudo apt-get install \
        build-essential \
        cmake \
        pkg-config \
        python3-dev \
        python3-gi \
        gir1.2-gstreamer-1.0 \
        gir1.2-gst-plugins-base-1.0 \
        gstreamer1.0-tools \
        gstreamer1.0-plugins-base \
        gstreamer1.0-plugins-good \
        gstreamer1.0-plugins-bad \
        gstreamer1.0-plugins-ugly \
        gstreamer1.0-python3-plugin-loader \
        libgirepository1.0-dev \
        libgstreamer1.0-dev \
        libcairo2-dev \
        libpango1.0-dev \
        libjpeg-dev \
        libgif-dev \
        librsvg2-dev
    ```

## MacOS

- Install Homebrew:
    ```
    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    ```

- Install OS packages:
    ```
    brew install \
        autoconf \
        automake \
        coreutils \
        cmake \
        pkg-config \
        python@3.7 \
        pygobject3 \
        gtk+3 \
        gstreamer \
        gst-plugins-base \
        gst-plugins-good \
        gst-plugins-ugly \
        gst-python \
        cairo \
        py3cairo
    ```

## Windows

- Go to http://www.msys2.org/ and download the x86_64 installer. Follow the instructions on the page for setting up the basic environment.
- Run C:\msys64\mingw64.exe and execute package manager:
    ```
    pacman -Suy
    pacman -S \
        python3 \
        python3-pip \
        python-devel \
        git \
        make \
        automake \
        cmake \
        mingw-w64-x86_64-pkg-config \
        mingw-w64-x86_64-lzo2 \
        mingw-w64-x86_64-gcc \
        mingw-w64-x86_64-gtk3 \
        mingw-w64-x86_64-python3 \
        mingw-w64-x86_64-python3-gobject \
        mingw-w64-x86_64-python-cairo \
        mingw-w64-x86_64-python-numpy \
        mingw-w64-x86_64-python-wheel \
        mingw-w64-x86_64-python-pkginfo \
        mingw-w64-x86_64-cairo \
        mingw-w64-x86_64-gst-devtools \
        mingw-w64-x86_64-gst-plugins-good \
        mingw-w64-x86_64-glib2 \
        mingw-w64-x86_64-gtk2 \
        mingw-w64-x86_64-gst-python \
        mingw-w64-x86_64-toolchain
    ```
