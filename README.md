Install scone:

* Add [pike repository](http://pike.esi.uclm.es/)
* sudo apt install scone

To extend scone KB with your own knowledge:

    my-project$ cp /usr/share/scone/scone-start.lisp .


Modify your `scone-start.lisp` including your knowledge files:

    (load "/usr/share/scone/scone-loader.lisp")
    (scone "1.0.0")
    (load-kb "core.lisp")

    (load "my-knowledge.lisp")


Launch scone:

    my-project$ sbcl --load scone-start.lisp


In the SBCL prompt execute:


    * (is-x-a-y? {Clyde} {elephant})
    :YES


**This repository is an example of all of this. Clone it**