# Welcome to MkDocs

{% include "Django.md" %}


![Placeholder](https://dummyimage.com/600x400/eee/aaa){ align=left }
jbhyjvjyvjyfuyfuyfuyy gvyufuygyuiguiygiugdd vwcvacv vfdawsdv 
vfyufguyvuyvjvjvjv



For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

`++ctrl+alt+del++`

``` { .js .annotate }
document$.subscribe(function() { // (1)
  var tables = document.querySelectorAll(/* (2) */ "article table")
  tables.forEach(function(table) {
    new Tablesort(table)
  })
})
```

1. ...
2. ...


``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```



=== "C"

    ``` c
    #include <stdio.h>

    int main(void) {
      printf("Hello world!\n");
      return 0;
    }
    ```

=== "C++"

    ``` c++
    #include <iostream>

    int main(void) {
      std::cout << "Hello world!" << std::endl;
      return 0;
    }
    ```



cds



| Method      | Description                          |
| ----------- | ------------------------------------ |
| `GET`       | :material-check:     Fetch resource  |
| `PUT`       | :material-check-all: Update resource |
| `DELETE`    | :material-close:     Delete resource |


dcwscw





!!! example

    === "Unordered List"

        _Example_:

        ``` markdown
        * Sed sagittis eleifend rutrum
        * Donec vitae suscipit est
        * Nulla tempor lobortis orci
        ```

        _Result_:

        * Sed sagittis eleifend rutrum
        * Donec vitae suscipit est
        * Nulla tempor lobortis orci

    === "Ordered List"

        _Example_:

        ``` markdown
        1. Sed sagittis eleifend rutrum
        2. Donec vitae suscipit est
        3. Nulla tempor lobortis orci
        ```

        _Result_:

        1. Sed sagittis eleifend rutrum
        2. Donec vitae suscipit est
        3. Nulla tempor lobortis orci




```python hl_lines="2 3"
# https://packaging.python.org/guides/distributing-packages-using-setuptools/
# python -m pip install -U wheel
# from distutils.core import
from setuptools import Extension, setup, find_packages
from Cython.Build import cythonize  # (1)


# setup(
#    name='Hello world app',
#    ext_modules=cythonize("hello.pyz"),
# )
```

```c++

#include <iostream>
#include <cstdlib>
#include <conio.h>
using namespace std;
int main()
{
    string str = "";
    while(1){
        char c = getche();
        if(c == '\r') break;
        str.push_back(c);
    }
    int size = str.size();
    for (int i = 0; i < size; i++)
    {
        int c = str[i];
        if(i == 0)
            str[0] -=32;
        if (c == ' ')
            str[i + 1] -=32;
    }
    system("PAUSE");
}
```