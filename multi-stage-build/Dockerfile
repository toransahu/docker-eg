# syntax=docker/dockerfile:1
FROM alpine:latest AS builder
RUN apk --no-cache add build-base

FROM builder AS build1
RUN touch file1

# the last FROM statement is the final base image
FROM builder AS build2
RUN touch file2
