# Docker_Lessons
Repository for Docker lessons.

## Homework1 usage:
1) **Easy.**
```
cd Homework1/Easy/
git clone https://github.com/pallets/flask.git
docker build -t <name>:<tag> .
docker run -ti -p XXXX:5000 <name>:<tag>
```
2) **Hard.**
```
cd Homework1/Hard/
git clone https://github.com/pallets/flask.git
docker build -t <name>:<tag> .
docker run -ti -p XXXX:5000 <name>:<tag>
```
3) **Extra.**
```
cd Homework1/Extra/
docker build -t <name>:<tag> .
docker run -ti -p XXXX:80 <name>:<tag>
```
