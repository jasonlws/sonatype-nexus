# Docker Image - Sonatype Nexus Repository

## What is Sonatype Nexus Repository

Sonatype Nexus Repository - Smart repository to manage and build artifacts, trusted by more than 150K orgranizations

## What is jasonlws/nexus3

Based on the [official Nexus Repository Docker image](https://hub.docker.com/r/sonatype/nexus3/) from Sonatype, but

- Added a default password `P@ssw0rd`, so you don't need retrieve from admin.password file

## Usage

```bash
$ docker run --name jasonlws-nexus3 -p 8081:8081 -v /some/dir/nexus-data:/nexus-data -d jasonlws/nexus3:3.70.1-java8-ubi
```

### Docker Volume

Use a docker volume. Since docker volumes are persistent, a volume can be created specifically for this purpose. This is the recommended approach.

```bash
$ docker volume create nexus-data
$ docker run --name jasonlws-nexus3 -p 8081:8081 -v nexus-data:/nexus-data -d jasonlws/nexus3:3.70.1-java8-ubi
```

### Mount a Host directory

Mount a host directory as the volume. This is not portable, as it relies on the directory existing with correct permissions on the host. However it can be useful in certain situations where this volume needs to be assigned to certain specific underlying storage.

#### Linux

```bash
$ docker run --name jasonlws-nexus3 -p 8081:8081 -v /docker-compose/nexus-data:/nexus-data -d jasonlws/nexus3:3.70.1-java8-ubi
```

#### Windows

```bash
$ docker run --name jasonlws-nexus3 -p 8081:8081 -v ${PWD}//docker-compose//nexus-data//:/nexus-data -d jasonlws/nexus3:3.70.1-java8-ubi
```

## Tags

| Tag | Based Image |
| :--- | :--- |
| 3.70.1-java8-ubi | Nexus 3.70.1 with Java 8 & Red Hat Universal Base Image 8 Minimal |

## Buidling the Sonatype Nexus Repository image

To build a docker image from the [Dockerfile](./Dockerfile)

```bash
$ docker build --rm=true --tag=jasonlws/nexus3:3.70.1-java8-ubi .
```

## License

MIT - a permissive free software license originating at the Massachusetts Institute of Technology (MIT), it puts only very limited restriction on reuse and has, therefore, an excellent license compatibility. It permits reuse within proprietary software provided that all copies of the licensed software include a copy of the MIT License terms and the copyright notice.

Check the [LICENSE file](https://github.com/jasonlws/sonatype-nexus/blob/master/LICENSE) for more details.