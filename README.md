# What is this?

Docker images for analytics environment
- Jupyter notebook
- MLflow
- PostgreSQL

I am developing my battlefield based on the great article by Danny Janz
https://towardsdatascience.com/containerize-your-whole-data-science-environment-or-anything-you-want-with-docker-compose-e962b8ce8ce5


# How to use this?

1. Download repository and update submodules
```
git clone https://github.com/not-so-fat/battlefield.git
cd battlefield
git submodule update --init --recursive
```

2. Edit docker-compose.yml
- Edit "<ENTER YOUR USERID>"
- Edit "<ENTER YOUR NOTEBOOK DIRECTORY>"

3. Build image

```
docker-compose build
```

4. Run image

```
docker-compose up
```

5. Develop your experiments on localhost:8888 / monitor experiments on localhost:5000
