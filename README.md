# TIL
## Miscellaneous things I learn throughout my day that I want to remember.

Circular imports in Python can be avoided with "import module.module" instead of "from module.module import function"
(Solves ImportError: cannot import name function)

Python subprocess checking the output of a django manage.py command:
```
import subprocess
subprocess.check_output(['python', 'manage.py', 'show_urls'])
```


Strip newline(s) at end of file then split the file by middle newlines:
```
for line in data.rstrip('\n').split('\n'):
(Strip chars at beginning of string with lstrip.)
```

Check if a python module is being run directly:
```
if __name__ == '__main__':
    main()
```

Return index of last substring in a string:
```
str.rindex('substring')
```

DjangoJS exposes a list of site URLs by default at `http://localhost:8000/djangojs/init.js`

Restrict the action of an ng-click in AngularJS based on the state of a setting:
```
ng-click="settings.wafflesEnabled && doSomethingWithWaffles()"
```
