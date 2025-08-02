FROM rockylinux/rockylinux

RUN dnf update -y
RUN dnf install -y git curl

RUN curl https://get.volta.sh | bash -s -- --skip-setup
ENV VOLTA_HOME=/root/.volta
ENV PATH="$VOLTA_HOME/bin:$PATH"

WORKDIR /app

RUN volta install node
RUN volta install pnpm