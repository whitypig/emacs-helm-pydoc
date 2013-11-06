# helm-pydoc.el

## Introduction
`helm-pydoc.el` is pydoc helm interface


## Screenshot

![helm-pydoc](image/helm-pydoc.png)

![helm-pydoc-action](image/helm-pydoc-action.png)


## Requirements

* Emacs 24 or higher
* helm 1.0 or higher

## Installation

You can install `helm-pydoc.el` from [MELPA](http://melpa.milkbox.net/) with `package.el`

```
 M-x package-install helm-pydoc
```


## Basic Usage

#### `helm-pydoc`

`pydoc` with helm interface


## Actions

* Show module document
* View source code
* Import module statement
    * import module(Insert marked candidates)
    * from module import identifier
    * from module import identifier


## Sample Configuration

```elisp
(eval-after-load "python"
  '(progn
     (define-key pythom-mode-map (kbd "C-c C-d") 'helm-pydoc)))
```
