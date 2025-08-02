FROM rockylinux/rockylinux

RUN dnf update -y
RUN dnf install -y git
COPY --from=ghcr.io/astral-sh/uv:latest /uv /uvx /bin/

WORKDIR /app

ENV PYTHONPATH=/app/src