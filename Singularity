BootStrap: docker
From: boutiques/boutiques

%post
  pip install coveralls pytest pytest-runner
  pip install simplejson jsonschema gitpython PyGithub

%runscript
  cd ./tools/python/
  coverage run --source boutiques setup.py pytest
  coveralls

