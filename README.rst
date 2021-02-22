Test sphinx-extensions for the DIRAC documentation
==================================================

To generate the sphinx documentation: ::

 sphinx-build -a docs/  html/
 cd html
 python3 -m http.server
 http://0.0.0.0:8000/

See https://demo-sphinx-extensions-for-dirac.readthedocs.io/en/latest/

This bug report shows how to publish on github.io 
https://github.com/sphinx-doc/sphinx/issues/3382

suhailvs commented on Jul 30, 2018
update of @wxianxin ::

    Create an empty .nojekyll file in the root folder to turn off Jekyll.
    Create an index.html file in the root folder with contents:
    <meta http-equiv="refresh" content="0; url=./_build/html/index.html" />
    Run make html then add, commit and push the repo.
    In the GitHub Pages box in the project Settings page, choose to use master branch.
    Visit https://<username>.github.io/<repo>



Your site is ready to be published at https://coding-to-music.github.io/demo-sphinx-extensions-for-DIRAC


