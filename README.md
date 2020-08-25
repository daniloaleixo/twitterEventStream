
## Running 
```
# Building notebook
docker build -t my-notebook -f docker/Dockerfile .

# Running notebook
docker run --rm -p 8888:8888 -e JUPYTER_ENABLE_LAB=yes -v "$PWD":/home/jovyan/work my-notebook