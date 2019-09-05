# Emacs init.el file for Clojure

## Keyboard layout




| Cider-Commands | Windows-Handling | Code-Text |
| :---           |     :---:        |          ---: |
| F1:eval sexp   | F6:del-win       | F10:comment-code|
| F2:eval buffer | F7:ver-split     | F11:format-code |
| F3:eval all    | F8:hor-split     | F12:search-text |
| F4:set ns      | F9:full-screen   |      |
| F5:jack-in     |                  |       |

| Left-Side         | Middle               | Right-Side |
| :---              |     :---:            |          ---: |
| highlight-text:~~ | start-mark:C-<SPC>   | zoom-out:--|
| para-mode:QQ      | end-region:MOUSE-3   | zoom-in:== |
| select-all:AA     | kill-line:KK         | kill-searchs:\\\\|
| sidebar-toggle:ZZ | create-file:C-x C-f  | kill-non-core:''     |



## Compile Clojure sequence	With main file selected
	F5 cider-jack-in
	F4 cider-repl-set-ns
	F3 cider-ns-reload-all       : compile a project
	F2 cider-load-buffer         : when a file has changed
	F1 cider-eval-defun-at-point : whan a single s-expression has changed

## Normal Undo/Cut/Copy/Paste
	(cua-mode t)

## Tabs 	
	(centaur-tabs-mode t)  

## Pop-up buffer menu via Control + Left-Click
	(defun mouse-buffer-menu-alist (the-buffers) 

## Sparser mode-lines
	(setq-default mode-line-format

## Auto-saving files
	(run-with-idle-timer

## Normal 'Delete' button behavior
	(require 'delsel)

## Active window highlighted
	(hiwin-activate)  

## Ignore '/' as word boundary 
	(modify-syntax-entry ?\/ "'" clojure-mode-syntax-table) 

## Window commands
	F6 delete current window
	F7 add window below
	F8 add window to right

## Comment/UnComment
	F9

## Format Clojure
	F10

## Full Screen
	F11

## Ag-Search
	F12

## Kill line
	press "k" key twice quickly

## Zoom out
	press "-" key twice quickly	

## Zoom in  
	press "=" key twice quickly	


## Change dired-sidebar   
	press "^^" key twice quickly	

## Highlight symbol in file  
	press "'" key twice quickly	

## Toggle Paredit mode 
	press "qq" key twice quickly	

## Select entire buffer
	press "a" key twice quickly	

## Toggle sidebar   
	press "zz" key twice quickly	
