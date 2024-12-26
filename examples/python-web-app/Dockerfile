FROM Ubuntu

WORKDIR /app

COPY Devops /app
COPY requirement.txt /app

RUN apt-get update && \
apt-get install -y python3 python3-pip && \
pip install -r requirement.txt && \
cd Devops
ENTRYPOINT ["python3"]
cmd ["manage.py", "runserver", "0.0.0.0:8000"]





