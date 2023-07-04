* make clean

* sphinx-apidoc -o source/docs pkag
* make html



软件包的rst文件存放在 `source/docs`



`pkag` 软件包使用到了  相对路径导包

* 在 `__init__.py` 文件中，把要生成API的方法与函数都 import 进去

* `pkag.rst` 不会自动添加 Submodules 的rst文件，手动添加即可

  * 比如: 

    `pkag.rst` 下述内容手动添加

    ```rst
    .. toctree::
       :maxdepth: 4
    
       pkag.tools.rst
    ```

    

