# basic shell based on elvish

## install ipfs

```
cd /tmp
wget https://dist.ipfs.io/go-ipfs/v0.4.10/go-ipfs_v0.4.10_linux-amd64.tar.gz 
tar -xvf go-ipfs_v0.4.10_linux-amd64.tar.gz 
cd go-ipfs
sh install.sh
rm -rf ~/.ipfs
ipfs init
ipfs daemon &
ufw allow 4001
```

## golang

```
cd /tmp
wget https://storage.googleapis.com/golang/go1.8.3.linux-amd64.tar.gz
tar -xvf go1.8.3.linux-amd64.tar.gz
rm -rf /opt/go
mv go /opt/go
export GOROOT=/opt/go
export GOPATH=/opt/goproj
export PATH=$GOPATH/bin:$GOROOT/bin:$PATH
go get github.com/elves/elvish
/opt/goproj/bin/elvish

```

## docker

```
cd /tmp
rm -f get-docker.sh
curl -fsSL get.docker.com -o get-docker.sh
sh get-docker.sh
```
