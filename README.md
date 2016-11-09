To extend scone KB with your own knowledge::

    $ sudo apt install scone
    my-project$ cp /usr/share/scone/scone-start.lisp .


Modify your `scone-start.lisp` including your knowledge files::

    (load "/usr/share/scone/scone-loader.lisp")
    (scone "1.0.0")
    (load-kb "core.lisp")

    (load-kb "my-knowledge.lisp")


Launch scone::

    my-project$ sbcl --load scone-start.lisp
