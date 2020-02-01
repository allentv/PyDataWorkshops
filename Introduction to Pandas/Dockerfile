FROM python:3.7.2

WORKDIR /opt/code

COPY Pipfile* ./

RUN pip install --upgrade pip && pip install pipenv
RUN pipenv sync

ENTRYPOINT pipenv run jupyter lab --ip='0.0.0.0' --no-browser --allow-root
