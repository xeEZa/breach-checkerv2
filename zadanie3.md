##zad1
docker inspect --format '{{json .Config.Labels}}' miron-rokita-frontend:v1
{"autor":"Miron Rokita,","data":"2026-10-14","maintainer":"miron.rokita@example.com,"}

PS D:\PolitechnikaPoznanska\MetodyWirtualizacji\breach-checker> docker history miron-rokita-frontend:v1
IMAGE          CREATED          CREATED BY                                      SIZE      COMMENT
f4e61370457c   11 minutes ago   EXPOSE [80/tcp]                                 0B        buildkit.dockerfile.v0
<missing>      11 minutes ago   RUN /bin/sh -c htmlhint /usr/share/nginx/htm…   4.1kB     buildkit.dockerfile.v0
<missing>      11 minutes ago   COPY . /usr/share/nginx/html # buildkit         32.8kB    buildkit.dockerfile.v0
<missing>      11 minutes ago   RUN /bin/sh -c apk add --no-cache nodejs npm…   99.4MB    buildkit.dockerfile.v0
<missing>      11 minutes ago   LABEL maintainer=miron.rokita@example.com, a…   0B        buildkit.dockerfile.v0
<missing>      3 days ago       RUN /bin/sh -c set -x     && apkArch="$(cat …   52.4MB    buildkit.dockerfile.v0
<missing>      3 days ago       ENV ACME_VERSION=0.4.2                          0B        buildkit.dockerfile.v0
<missing>      3 days ago       ENV NJS_RELEASE=1                               0B        buildkit.dockerfile.v0
<missing>      3 days ago       ENV NJS_VERSION=1.0.2                           0B        buildkit.dockerfile.v0
<missing>      3 days ago       CMD ["nginx" "-g" "daemon off;"]                0B        buildkit.dockerfile.v0
<missing>      3 days ago       STOPSIGNAL SIGQUIT                              0B        buildkit.dockerfile.v0
<missing>      3 days ago       EXPOSE map[80/tcp:{}]                           0B        buildkit.dockerfile.v0
<missing>      3 days ago       ENTRYPOINT ["/docker-entrypoint.sh"]            0B        buildkit.dockerfile.v0
<missing>      3 days ago       COPY 30-tune-worker-processes.sh /docker-ent…   16.4kB    buildkit.dockerfile.v0
<missing>      3 days ago       COPY 20-envsubst-on-templates.sh /docker-ent…   12.3kB    buildkit.dockerfile.v0
<missing>      3 days ago       COPY 15-local-resolvers.envsh /docker-entryp…   12.3kB    buildkit.dockerfile.v0
<missing>      3 days ago       COPY 10-listen-on-ipv6-by-default.sh /docker…   12.3kB    buildkit.dockerfile.v0
<missing>      3 days ago       COPY docker-entrypoint.sh / # buildkit          8.19kB    buildkit.dockerfile.v0
<missing>      3 days ago       RUN /bin/sh -c set -x     && addgroup -g 101…   11.9MB    buildkit.dockerfile.v0
<missing>      3 days ago       ENV DYNPKG_RELEASE=1                            0B        buildkit.dockerfile.v0
<missing>      3 days ago       ENV PKG_RELEASE=1                               0B        buildkit.dockerfile.v0
<missing>      3 days ago       ENV NGINX_VERSION=1.31.10                       0B        buildkit.dockerfile.v0
<missing>      3 days ago       LABEL maintainer=NGINX Docker Maintainers <d…   0B        buildkit.dockerfile.v0
<missing>      3 weeks ago      CMD ["/bin/sh"]                                 0B        buildkit.dockerfile.v0
<missing>      3 weeks ago      ADD alpine-minirootfs-3.24.4-x86_64.tar.gz /…   9.09MB    buildkit.dockerfile.v0
