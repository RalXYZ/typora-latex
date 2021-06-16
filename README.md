# Typora LaTeX

![ski.png](https://i.loli.net/2021/06/17/l8HaKEgYj9zxF1O.png)  

A LaTeX-style theme for Typora.  

## Current Issue

Currently, this theme can only work in English Typora files.  
The comparability to Chinese characters is poor, which will be fixed in the future.  

## Usage

### Get CSS File

Choose between the following two options:  

1. Get the CSS file from *Release*. 
2. Build by yourself, following the steps in "Build" section.

### Deployment

Open Typora.  
In `File -> Preferences... -> Appearance`, click `Open Theme Folder` button. Copy the CSS file of your operating system to this folder.  

## Build

Firstly, make sure you have installed `ruby sass`:  
```shell
sudo apt install ruby
sudo apt install sass
```

Then, grant execution permission to `make.sh`:  
```shell
chmod u+x make.sh
```

Finally, run the shell script:  
```shell
./make.sh
```

You can then find the generated CSS files in `./latex-theme`.  

## Credit

This work is based on [Keldos-Li/typora-latex-theme](https://github.com/Keldos-Li/typora-latex-theme).  

Changes between `2fd2fc8` of `Keldos-Li/typora-latex-theme` and the commit which creates this README file in this repository have the following changes:  

- Remove files unrelated to the theme CSS
- Merge the Windows and macOS CSS files together, using SCSS and shell script to generate the separated two files, which is almost the same compared to the files in `Keldos-Li/typora-latex-theme`, except putting all CSS code in one file and removed some comments.  

