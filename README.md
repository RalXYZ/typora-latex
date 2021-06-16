# Typora LaTeX

![ski.png](https://i.loli.net/2021/06/17/l8HaKEgYj9zxF1O.png)  

A LaTeX-style theme for Typora. Supports Chinese characters on Windows and macOS.  

## Usage

### Get CSS File

Choose between the following two options:  

1. Get CSS file from *Releases*. 
2. Build by yourself, following the steps listed in "Build" section below.

### Deployment

Open Typora.  
In `File -> Preferences... -> Appearance`, click `Open Theme Folder` button. Copy the CSS file of your operating system to this folder.  

## Build

Firstly, make sure you have installed `ruby sass`:  
```shell
sudo apt install ruby
sudo apt install sass
```

Then, run the shell script:  
```shell
./make.sh
```

You can then find the generated CSS files in `./latex-theme`.  

## Current Issue

Currently, this theme can display Latin characters on every platform. Chinese characters could be correctly displayed on Windows and macOS.  
The support of Chinese characters on Linux is poor, which will be fixed in the future.  

## Credit

This project is based on [Keldos-Li/typora-latex-theme](https://github.com/Keldos-Li/typora-latex-theme).  

The commit which creates this README file in this repository has the following changes, compared to `2fd2fc8` of `Keldos-Li/typora-latex-theme`:  

- Remove files unrelated to the theme CSS
- Merge Windows and macOS CSS files together, using SCSS and shell script to generate CSS files. And the resulting CSS files are almost the same compared to the files in `Keldos-Li/typora-latex-theme`, except putting all CSS code in one file and removed some comments.  

