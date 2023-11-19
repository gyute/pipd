FROM python:3.11.6-bookworm

ENV PYTHONUNBUFFERED=1

WORKDIR /pipd

RUN pip install fastapi uvicorn[standard] pydantic motor

ENTRYPOINT ["uvicorn", "app.mon:app", "--host", "0.0.0.0", "--reload"]
