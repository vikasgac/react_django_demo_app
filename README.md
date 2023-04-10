# react_django_demo_app
A demo app for React and Django Deployment

docker-compose down
docker-compose up -d

-----steps to be followed to deploy a sample react-django app using dockerfile------

1.git clone https://github.com/vickscool/react_django_demo_app.git
2.mkdir react-django-app
3.cd react-django-app
4.update the dockerfile with content from this repository 
5.Build the image from dockerfile : docker build . -t react-django-app:latest
6.Check the images : docker images
7.Run the container from build image : docker run -d -p 8000:8000 react-django-app:latest
8.Enable port 8000 in inbound security group of VM you are working on . For  ex. from AWS Console
