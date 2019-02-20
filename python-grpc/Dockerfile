FROM python:3.7-alpine as base

FROM base
ENV GRPC_PYTHON_VERSION 1.15.0
RUN apk add --update --no-cache \
      gcc \
      linux-headers \
      make \
      musl-dev \
      python-dev \
      g++ \
    && python -m pip install --upgrade pip \
    && pip install grpcio==${GRPC_PYTHON_VERSION} \
      grpcio-tools==${GRPC_PYTHON_VERSION} \
      grpcio-reflection==${GRPC_PYTHON_VERSION} \
      grpcio-health-checking==${GRPC_PYTHON_VERSION} \
      grpcio-testing==${GRPC_PYTHON_VERSION}
