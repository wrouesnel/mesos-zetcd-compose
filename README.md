# Usage

Check out the zetcd project to your GOPATH:

```
go get -v github.com/coreos/zetcd
```

Note: to make this work you currently need zetcd from my own branch, so do the
following:
```
cd $GOPATH/src/github.com/coreos/zetcd
git remote add wrouesnel https://github.com/wrouesnel/zetcd
git fetch --all
git checkout naive_fix_watches
```

Run the build script to get a static binary:
```
zetcd/build.sh
```

Then docker-compose up:
```
docker-compose up --force-recreate --build
```
