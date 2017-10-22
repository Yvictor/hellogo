# hellogo
play go~~~

## Install GO
```
#add to ~/.bashrc
# go
export GOROOT="$HOME/Gos/go1.x.x"
export GOPATH="$HOME/Gos/pkg1.x.x"
export PATH="$GOROOT/bin:$PATH"

wget https://storage.googleapis.com/golang/go*.tar.gz
tar -C $HOME/Gos -xzf go*.tar.gz
```

## Install GO for jupyter
```
go get github.com/gopherdata/gophernotes
go install github.com/gopherdata/gophernotes
mkdir -p ~/.local/share/jupyter/kernels/gophernotes
cp $GOPATH/src/github.com/gopherdata/gophernotes/kernel/* ~/.local/share/jupyter/kernels/gophernotes

# add to ~/.bashrc
# gophernotes
export PATH="$PATH:$GOPATH/bin/"
```

