I fixed dependency nut I am unable to start the application
When I run 
    python tinyurl/manage.py test
I got:    
Traceback (most recent call last):
  File "/workspaces/urlShortener/tinyurl/manage.py", line 21, in <module>
    main()
  File "/workspaces/urlShortener/tinyurl/manage.py", line 17, in main
    execute_from_command_line(sys.argv)
  File "/usr/local/python/3.12.1/lib/python3.12/site-packages/django/core/management/__init__.py", line 443, in execute_from_command_line
    utility.execute()
  File "/usr/local/python/3.12.1/lib/python3.12/site-packages/django/core/management/__init__.py", line 417, in execute
    django.setup()
  File "/usr/local/python/3.12.1/lib/python3.12/site-packages/django/__init__.py", line 24, in setup
    apps.populate(settings.INSTALLED_APPS)
  File "/usr/local/python/3.12.1/lib/python3.12/site-packages/django/apps/registry.py", line 91, in populate
    app_config = AppConfig.create(entry)
                 ^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/python/3.12.1/lib/python3.12/site-packages/django/apps/config.py", line 193, in create
    import_module(entry)
  File "/usr/local/python/3.12.1/lib/python3.12/importlib/__init__.py", line 90, in import_module
    return _bootstrap._gcd_import(name[level:], package, level)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "<frozen importlib._bootstrap>", line 1387, in _gcd_import
  File "<frozen importlib._bootstrap>", line 1360, in _find_and_load
  File "<frozen importlib._bootstrap>", line 1324, in _find_and_load_unlocked
ModuleNotFoundError: No module named 'sass_processor'
@daitangio ➜ /workspaces/urlShortener (master) $ python tinyurl/manage.py 
Traceback (most recent call last):
  File "/workspaces/urlShortener/tinyurl/manage.py", line 21, in <module>
    main()
  File "/workspaces/urlShortener/tinyurl/manage.py", line 17, in main
    execute_from_command_line(sys.argv)
  File "/usr/local/python/3.12.1/lib/python3.12/site-packages/django/core/management/__init__.py", line 443, in execute_from_command_line
    utility.execute()
  File "/usr/local/python/3.12.1/lib/python3.12/site-packages/django/core/management/__init__.py", line 417, in execute
    django.setup()
  File "/usr/local/python/3.12.1/lib/python3.12/site-packages/django/__init__.py", line 24, in setup
    apps.populate(settings.INSTALLED_APPS)
  File "/usr/local/python/3.12.1/lib/python3.12/site-packages/django/apps/registry.py", line 91, in populate
    app_config = AppConfig.create(entry)
                 ^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/python/3.12.1/lib/python3.12/site-packages/django/apps/config.py", line 193, in create
    import_module(entry)
  File "/usr/local/python/3.12.1/lib/python3.12/importlib/__init__.py", line 90, in import_module
    return _bootstrap._gcd_import(name[level:], package, level)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "<frozen importlib._bootstrap>", line 1387, in _gcd_import
  File "<frozen importlib._bootstrap>", line 1360, in _find_and_load
  File "<frozen importlib._bootstrap>", line 1324, in _find_and_load_unlocked
ModuleNotFoundError: No module named 'sass_processor'

Can you fix the problem?