# Postgresql DB 서버 실행 cmd
# sudo docker run -d --name postgres16 -e POSTGRES_PASSWORD=password -p 5433:5432 postgres:16.4
###############################################
# Powershell 해당 Dockerfile 위치에서
# # 이미지 빌드
# docker build -t postgres-16-db .

# # 실행
# docker run -d -p 5433:5432 --name postgres-16-db postgres-16-db

# # psql terminal
# docker exec -it postgres-16-db psql -U postgres

# # ID 조회 후 중지
# docker ps 후
# docker stop [CONTAINER ID]
#
# # 컨테이터 삭제
# docker rm [CONTAINER ID]
###############################################

# PostgreSQL 16.4 공식 이미지 기반
FROM postgres:16.4

# 환경 변수 설정 (컨테이너 빌드 시 적용됨)
ENV POSTGRES_USER=postgres
ENV POSTGRES_PASSWORD=password

# PostgreSQL port open
EXPOSE 5433

# 볼륨 설정 (데이터 영속화)
VOLUME ["/var/lib/postgresql/data"]

# 기본 실행 명령어
CMD ["postgres"]