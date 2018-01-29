# emacs-new-buffer

[![Marmalade](https://img.shields.io/badge/marmalade-available-8A2A8B.svg)](https://marmalade-repo.org/packages/emacs-new-buffer)  
[![License](https://img.shields.io/badge/LICENSE-GPL%20v3.0-blue.svg)](https://www.gnu.org/licenses/gpl.html)

Quickly create new buffers to take notes and more

## Installation

### Manual

Save the file *emacs-new-buffer.el* to disk and add the directory containing it to `load-path` using a command in your *.emacs* file like:

    (add-to-list 'load-path "~/.emacs.d/")

The above line assumes that you've placed the file into the Emacs directory '.emacs.d'.

Start the package with:

    (require 'emacs-new-buffer)

### Marmalade

If you have Marmalade added as a repository to your Emacs, you can just install *emacs-new-buffer* with

    M-x package-install emacs-new-buffer RET

## Usage

Quickly create a buffer with name as current timestamp

    M-x emacs-new-buffer-now RET

Create a buffer with a specific file extension (hence specific major mode)

    M-x emacs-new-buffer-as RET
    
This is useful when used with a key-binding

    (global-set-key (kbd "C-x t") 'emacs-new-buffer-now)
    (global-set-key (kbd "C-x y") 'emacs-new-buffer-as)
