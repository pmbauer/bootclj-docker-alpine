#### What is this?
A Docker image packaging [boot-clj](http://boot-clj.com) JDK8, and Clojure 1.7.0

Based on Alpine Linux, it clocks in at smidge over 209 MB.

#### Example

```
# jump quickly to a repl
docker run --rm -it pmbauer/bootclj:2.2.0 repl

# build a jar for boot project in the current folder
docker run --net=host --rm -it -v $(pwd):/data pmbauer/bootclj:2.2.0 jar
```

#### License
```
Copyright 2015 Paul Bauer

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
```

#### Thanks to
* Vlad Frolov and his [docker-alpine-oraclejdk8](https://github.com/frol/docker-alpine-oraclejdk8) image
* David Yarwood and his [debian-based bootclj](https://github.com/adzerk-oss/boot-clj-docker-image) image
* Micha Niskin and Alan Dipert for boot-clj
