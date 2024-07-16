# About Sonatype Nexus Repository OSS

## What is Sonatype Nexus Repository OSS

Sonatype Nexus Repository - Smart repository to manage and build artifacts, trusted by more than 150K orgranizations. Nexus OSS, also known as Nexus Open Source Software, is a repository manager used for storing and managing artifacts such as libraries, dependencies, and Docker images. It ensures that artifacts are available and accessible to all members of your development team.

## Nexus Repository Supports Formats

Nexus Repository supports the repository formats listed below. 

| Format | Description |
| :--- | :--- |
| [APT](https://help.sonatype.com/en/apt-repositories.html) | Use Advanced Package Tool (APT) tools such as apt-get to access hosted Debian, Ubuntu and other Linux software packages. |
| [Bower](https://help.sonatype.com/en/bower-repositories.html) | Keep track of all your web site frontend development packages using Bower registries. Note that Bower format is not compatible with H2 or PostgreSQL databases. |
| [CocoaPods](https://help.sonatype.com/en/cocoapods-repositories.html) | Manager for CocoaPods packages (which might contain Swift code) and Objective-C Cocoa projects. Note that we do not support Apple's Swift package manager. |
| [Conan](https://help.sonatype.com/en/conan-repositories.html) | Share your C/C++ packages in a central repository. |
| [Conda](https://help.sonatype.com/en/conda-repositories.html) | Proxy Conda packages for languages such as Python, R, Ruby, Lua, Scala, Java, JavaScript, C/C++ and FORTRAN. |
| [Docker](https://help.sonatype.com/en/docker-registry.html) | Proxy popular Docker registries such as DockerHub and host your own private images securely. |
| [Git LFS](https://help.sonatype.com/en/git-lfs-repositories.html) | Store large files such as audio samples, videos, datasets, and graphics inside repositories and use simple text pointers to these inside your Git project. |
| [Go](https://help.sonatype.com/en/go-repositories.html) | Modernize your development process and store Go (golang) dependencies for fast, repeatable local builds. |
| [Helm](https://help.sonatype.com/en/helm-repositories.html) | Manage packages for Kubernetes by accessing Helm Charts in Helm repositories. |
| [Maven](https://help.sonatype.com/en/maven-repositories.html) | Leverage the most experienced Maven repository format product to host your private Java components and proxy defacto public repositories like Central using tooling such as Maven, Ant and Gradle. |
| [npm](https://help.sonatype.com/en/npm-registry.html) | Publish your javascript node.js projects to hosted registries and integrate dependencies from external JavaScript package registries. |
| [NuGet](https://help.sonatype.com/en/nuget-repositories.html) | Use NuGet client compatible tooling to push and install .Net packages. Development is easier using consolidated hosted and proxy registries. |
| [p2](https://help.sonatype.com/en/p2-repositories.html) | Proxy p2 format repositories for your Eclipse IDE and other Equinox based application dependencies. |
| [PyPI](https://help.sonatype.com/en/pypi-repositories.html) | Python development tools such as pip and twine can be used install and publish packages to PyPI repositories. |
| [R](https://help.sonatype.com/en/r-repositories.html) | Proxy packages from the official R registry and host your own packages. |
| [Raw](https://help.sonatype.com/en/raw-repositories.html) | A flexible format that does not enforce any type of layout enabling you to store and serve any type of binary content such as Maven sites over HTTP. |
| [RubyGems](https://help.sonatype.com/en/rubygems-repositories.html) | Host your own gems and proxy remote gem repositories like rubygems.org. |
| [Yum](https://help.sonatype.com/en/yum-repositories.html) | First class support for hosting and proxying your RPM distributions. |

## Set Up Your Environment

### Docker

Please refer to [docker](https://github.com/jasonlws/sonatype-nexus/tree/master/docker) folder.

### Docker Compose

Please refer to [docker-compose](https://github.com/jasonlws/sonatype-nexus/tree/master/docker-compose) folder.

### Vagrant

Please refer to [vagrant](https://github.com/jasonlws/sonatype-nexus/tree/master/vagrant) folder.

## License

MIT - a permissive free software license originating at the Massachusetts Institute of Technology (MIT), it puts only very limited restriction on reuse and has, therefore, an excellent license compatibility. It permits reuse within proprietary software provided that all copies of the licensed software include a copy of the MIT License terms and the copyright notice.

Check the [LICENSE file](https://github.com/jasonlws/sonatype-nexus/blob/master/LICENSE) for more details.