docker-golang-devel
===================

Go language container (golang) that can run "go service scripts".

Softare versions:

- Go 1.2.2 (it seems that Go 1.3 is not working properly for debugging https://code.google.com/p/go/issues/detail?id=8098)

Run
---

Change `/<user-home-dir>/go` with the absolute path of your src parent directory. 

	$ docker run -v="/<user-home-dir>/go:/go:rw" jordi/golang:run

If you edit and save your source files, they will remain on your host after the container has been stopped or killed.

Pull
----

	$ docker pull jordi/golang:run

Build
-----

`git clone` this project, cd into it, and:

	$ docker build -t golang:run .

