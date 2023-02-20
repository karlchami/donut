FROM python:3.10.2-buster AS builder

COPY . /donut

WORKDIR /donut

RUN pip install poetry
RUN poetry config virtualenvs.create false
RUN poetry export -f requirements.txt > requirements.txt

FROM python:3.10.2-slim-buster

EXPOSE 8000

ENV PORT 8000
ENV HOST "0.0.0.0"

COPY --from=builder /donut /donut

WORKDIR /donut

RUN pip install -r requirements.txt

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]