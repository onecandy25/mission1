# Mission 1 - Docker Web Server

## 개요
Docker와 Nginx를 사용하여 간단한 정적 웹 페이지를 실행하는 프로젝트입니다.

## 실행 환경
- WSL2 Ubuntu
- Docker Desktop
- Nginx Alpine 이미지

## 파일 구성
- `index.html` : 웹 브라우저에 표시될 HTML 파일
- `Dockerfile` : Docker 이미지를 만들기 위한 설정 파일
- `README.md` : 프로젝트 설명 문서

## Docker 이미지 빌드

```bash
docker build -t mission1-web .
docker run -d --name mission1-web -p 8080:80 mission1-web
docker ps
