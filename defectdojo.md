# DefectDojo
docker run -it -p 8000:8000 appsecpipeline/django-defectdojo bash -c "export LOAD_SAMPLE_DATA=True && bash /opt/django-DefectDojo/docker/docker-startup.bash"

http://localhost:8000 with the default credentials (user: admin, password: admin)
