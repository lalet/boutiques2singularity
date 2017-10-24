BootStrap: docker
From: boutiques/boutiques

%post
  pip install coveralls pytest pytest-runner boutiques
  pip install simplejson jsonschema gitpython PyGithub

%runscript
  cd /usr/local/
  git clone https://github.com/boutiques/boutiques.git
  cd boutiques/tools/python
  coverage run --source boutiques setup.py pytest
  coveralls

