build:
	docker build -t "intro_to_pandas" .

start:
	docker run --rm -p 8888:8888 -e JUPYTER_ENABLE_LAB=yes -v "$(PWD)":/opt/code --name="intro-to-pandas-container" "intro_to_pandas"

stop:
	docker kill "intro-to-pandas-container"
