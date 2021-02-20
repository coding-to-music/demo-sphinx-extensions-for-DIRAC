Test sphinx-extensions for the DIRAC documentation
==================================================

To generate the sphinx documentation:

 sphinx-build -a docs/  html/
 cd html
 python3 -m http.server
 http://0.0.0.0:8000/

See https://demo-sphinx-extensions-for-dirac.readthedocs.io/en/latest/

