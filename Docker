FROM python:3.8

ENV PYTHONUNBUFFERED 1

RUN mkdir /Hospital-management-system-
WORKDIR /Hospital-management-system-

COPY requirements.txt /Hospital-management-system-/
RUN pip install --upgrade pip wheel
RUN pip install -r requirements.txt

COPY . /Hospital-management-system-/

CMD ["python", "-m", "flask", "run", "--host=0.0.0.0", "--port=5000"]
