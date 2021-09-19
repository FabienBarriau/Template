========
How to create a python repository with necessary CI/CD tools
========

Create a repo with pyscaffold::

  conda create --name template python=3.9
  pip install pyscaffold
  putup template
  pip install tox
  
Optional

Connect to github with github cli::

  conda install gh --channel conda-forge
  gh auth login
  gh repo create template
  git branch -M main
  git push -u origin main
  

Specificity

copy/paste .gitignore and tox.ini of this repo


========
New tox env
========

* format

  * isort
  * black
  
* lint

  * flake8
  * pylint
  
* type

  * mypy
  
* security

  * bandit
  
* mutation_testing

  * mutmut


  
  
  


