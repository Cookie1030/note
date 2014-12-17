Log 
=====

  yum install -y zlib-devel
  curl -s https://raw.githubusercontent.com/oscm/shell/master/compiler/gcc.sh | bash
  curl -s https://raw.githubusercontent.com/oscm/shell/master/lang/python/python3.tarball.sh | bash
  
  cd /usr/local/src
  git clone https://github.com/netkiller/logging.git
  cd logging
  python3 setup.py sdist
  python3 setup.py install --prefix=/srv/logging
