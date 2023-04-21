nome-projeto = nome-do-projeto 
build:
	docker build -t $(nome-projeto) .
run:
	docker run -it -v $(shell pwd):/app $(nome-projeto):latest
bnote:
	docker build -t neural-note -f Dockerfile.jupyter .
note:
	docker run -p 10000:8888 -v $(shell pwd):/app neural-note:latest

