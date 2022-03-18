# Feihong's J quickstart

## Installation

### Mac

    wget http://www.jsoftware.com/download/j903/install/j903_mac64.zip
    unzip j903_mac64.zip
    mv j903 ~/Applications
    ~/Applications/j903/bin/jconsole
    install 'qtide'
    ^D
    ln -s ~/Applications/j903/bin/jqt /usr/local/bin/jqt

### Linux

    curl http://www.jsoftware.com/download/j903/install/j903_linux64.tar.gz | tar xvz -C ~/opt
    ~/opt/j903/bin/jconsole
    install 'qtide'
    ^D
    cat "alias jqt='~/opt/j903/jqt.sh'" >> ~/.profile
    source ~/.profile

### Install useful packages (inside J)

    install 'labs/labs'
    install 'graphics/plot'
    install 'graphics/viewmat'
    install 'convert/json'

### Install J Jupyter kernel

    curl https://github.com/martin-saurer/jkernel/archive/refs/tags/3.2.4.tar.gz | tar xvz
    cd jkernel-3.2.4
    python setup.py install
    cd ..
    rm -rf jkernel-3.2.4

## Commands

Run J's Qt IDE

    jqt

## Links

- [System/Installation/J903/Zips](https://code.jsoftware.com/wiki/System/Installation/J903/Zips)
- [Qt IDE install](https://code.jsoftware.com/wiki/Guides/Qt_IDE/Install)
- [J kernel for Jupyter](https://github.com/martin-saurer/jkernel)
