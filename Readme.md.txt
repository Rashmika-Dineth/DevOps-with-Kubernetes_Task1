## Deployment with Docker ## 

PS F:\Knowledge Improvements\Kubernetes\Task1> docker build -t my-node-app .
[+] Building 1.1s (10/10) FINISHED                                                                 docker:desktop-linux
 => [internal] load build definition from Dockerfile                                                               0.0s
 => => transferring dockerfile: 137B                                                                               0.0s
 => [internal] load metadata for docker.io/library/node:alpine                                                     0.6s
 => [internal] load .dockerignore                                                                                  0.0s
 => => transferring context: 2B                                                                                    0.0s
 => [1/5] FROM docker.io/library/node:alpine@sha256:d03e75e7ba1385c2944f4cc374eb5abe0715234f87da5121dbd64f7262ad1  0.1s
 => => resolve docker.io/library/node:alpine@sha256:d03e75e7ba1385c2944f4cc374eb5abe0715234f87da5121dbd64f7262ad1  0.1s
 => [internal] load build context                                                                                  0.1s
 => => transferring context: 4.44kB                                                                                0.0s
 => CACHED [2/5] WORKDIR /usr/src/app                                                                              0.0s
 => CACHED [3/5] COPY package* ./                                                                                  0.0s
 => CACHED [4/5] RUN npm ci                                                                                        0.0s
 => CACHED [5/5] COPY . .                                                                                          0.0s
 => exporting to image                                                                                             0.2s
 => => exporting layers                                                                                            0.0s
 => => exporting manifest sha256:a5b12075a8faf77e43398ac58c57569ea5c89df5411c85008acf3170c5be531c                  0.0s
 => => exporting config sha256:91c98b15c42db2097228a3192a18dd410d2f6957aea1c7ff2d9dded47e9544bb                    0.0s
 => => exporting attestation manifest sha256:46a3fec55d4ef08807b768607cdf61c17f2185a8a9f9ef6289666a2dd63b1c55      0.0s
 => => exporting manifest list sha256:1e330305193e79b18892c041bbcd809236a6a8507d18c63beb26c72fa5f0b4a1             0.0s
 => => naming to docker.io/library/my-node-app:latest                                                              0.0s
 => => unpacking to docker.io/library/my-node-app:latest                                                           0.0s
[+] Building 1.1s (10/10) FINISHED                                                                 docker:desktop-linux
 => [internal] load build definition from Dockerfile                                                               0.0s
 => => transferring dockerfile: 137B                                                                               0.0s
 => [internal] load metadata for docker.io/library/node:alpine                                                     0.5s
 => [internal] load .dockerignore                                                                                  0.0s
 => => transferring context: 2B                                                                                    0.0s
 => [1/5] FROM docker.io/library/node:alpine@sha256:d03e75e7ba1385c2944f4cc374eb5abe0715234f87da5121dbd64f7262ad1  0.1s
 => => resolve docker.io/library/node:alpine@sha256:d03e75e7ba1385c2944f4cc374eb5abe0715234f87da5121dbd64f7262ad1  0.1s
 => [internal] load build context                                                                                  0.0s
 => => transferring context: 4.44kB                                                                                0.0s
 => CACHED [2/5] WORKDIR /usr/src/app                                                                              0.0s
 => CACHED [3/5] COPY package* ./                                                                                  0.0s
 => CACHED [4/5] RUN npm ci                                                                                        0.0s
 => CACHED [5/5] COPY . .                                                                                          0.0s
 => exporting to image                                                                                             0.2s
 => => exporting layers                                                                                            0.0s
 => => exporting manifest sha256:a5b12075a8faf77e43398ac58c57569ea5c89df5411c85008acf3170c5be531c                  0.0s
 => => exporting config sha256:91c98b15c42db2097228a3192a18dd410d2f6957aea1c7ff2d9dded47e9544bb                    0.0s
 => => exporting attestation manifest sha256:ecca8b96b14bf1cf957aa90a0d2796aeea1b43c57de58e1ce7600da5413e5a36      0.1s
 => => exporting manifest list sha256:15bdfb2a528caedc754bc619763b90b5ccb71276559f55fd07fda54b19fa03df             0.0s
 => => naming to docker.io/library/my-node-app:latest                                                              0.0s
 => => unpacking to docker.io/library/my-node-app:latest                                                           0.0s
[+] Building 48.2s (11/11) FINISHED                                                                                                      docker:desktop-linux
 => [internal] load build definition from Dockerfile                                                                                                     0.1s
 => => transferring dockerfile: 451B                                                                                                                     0.0s
 => [internal] load metadata for docker.io/library/node:16                                                                                               1.9s
 => [auth] library/node:pull token for registry-1.docker.io                                                                                              0.0s
 => [internal] load .dockerignore                                                                                                                        0.1s
 => => transferring context: 2B                                                                                                                          0.0s
 => [1/5] FROM docker.io/library/node:16@sha256:f77a1aef2da8d83e45ec990f45df50f1a286c5fe8bbfb8c6e4246c6389705c0b                                        35.4s
 => => resolve docker.io/library/node:16@sha256:f77a1aef2da8d83e45ec990f45df50f1a286c5fe8bbfb8c6e4246c6389705c0b                                         0.1s
 => => sha256:ee7d78be1eb92caf6ae84fc3af736b23eca018d5dedc967ae5bdee6d7082403b 450B / 450B                                                               0.2s
 => => sha256:ca266fd6192108b67fb57b74753a8c4ca5d8bd458baae3d4df7ce9f42dedcc1d 2.27MB / 2.27MB                                                           0.5s
 => => sha256:0e421f66aff42bb069dffc26af6d132194b22a1082b08c5ef7cd69c627783c04 34.79MB / 34.79MB                                                         9.2s
 => => sha256:ae3b95bbaa61ce24cefdd89e7c74d6fbd7713b2bcae93af47063d06bd7e02172 4.20kB / 4.20kB                                                           0.6s
 => => sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e 191.90MB / 191.90MB                                                      28.0s
 => => sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5 51.89MB / 51.89MB                                                        16.8s
 => => sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454 17.58MB / 17.58MB                                                         4.1s
 => => sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017 50.50MB / 50.50MB                                                        12.3s
 => => extracting sha256:311da6c465ea1576925360eba391bcd32dece9be95960a0bc9ffcb25fe712017                                                                2.8s
 => => extracting sha256:7e9bf114588c05b2df612b083b96582f3b8dbf51647aa6138a50d09d42df2454                                                                0.7s
 => => extracting sha256:ffd9397e94b74abcb54e514f1430e00f604328d1f895eadbd482f08cc02444e5                                                                2.9s
 => => extracting sha256:513d779256048c961239af5f500589330546b072775217272e19ffae1635e98e                                                                4.9s
 => => extracting sha256:ae3b95bbaa61ce24cefdd89e7c74d6fbd7713b2bcae93af47063d06bd7e02172                                                                0.0s
 => => extracting sha256:0e421f66aff42bb069dffc26af6d132194b22a1082b08c5ef7cd69c627783c04                                                                1.5s
 => => extracting sha256:ca266fd6192108b67fb57b74753a8c4ca5d8bd458baae3d4df7ce9f42dedcc1d                                                                0.1s
 => => extracting sha256:ee7d78be1eb92caf6ae84fc3af736b23eca018d5dedc967ae5bdee6d7082403b                                                                0.0s
 => [internal] load build context                                                                                                                        0.1s
 => => transferring context: 4.87kB                                                                                                                      0.0s
 => [2/5] WORKDIR /usr/src/app                                                                                                                           5.9s
 => [3/5] COPY package*.json ./                                                                                                                          0.1s
 => [4/5] RUN npm install                                                                                                                                2.6s
 => [5/5] COPY . .                                                                                                                                       0.9s
 => exporting to image                                                                                                                                   0.8s
 => => exporting layers                                                                                                                                  0.5s
 => => exporting manifest sha256:7f4a5ddd6c8158f95e6abd4703b43d25d3017ccfd52f46ac6f63832e3d375029                                                        0.0s
 => => exporting config sha256:6209bc75447afc396dabf1d97b272db99b8a8e6a045e0d28552cc0b1fb3f05d5                                                          0.0s
 => => exporting attestation manifest sha256:8f5e66616541d271cedaa233a8f32285da0932f1c2767eee7cdbddabf60f58cc                                            0.0s
 => => exporting manifest list sha256:8e214649ee636c46b7251faba920383df08f9b0f9e49ad571a50a876cbfb2636                                                   0.0s
 => => naming to docker.io/library/my-node-app:latest                                                                                                    0.0s
 => => unpacking to docker.io/library/my-node-app:latest                                                                                                 0.2s
PS F:\Knowledge Improvements\Kubernetes\Task1> docker run -p 3000:3000 my-node-app
2024-12-04T09:19:58.129Z   UPJ3AnzKwQMveCQXP1jVUvuaOReWdhGj
2024-12-04T09:20:03.134Z   UPJ3AnzKwQMveCQXP1jVUvuaOReWdhGj
2024-12-04T09:20:08.135Z   UPJ3AnzKwQMveCQXP1jVUvuaOReWdhGj
2024-12-04T09:20:13.136Z   UPJ3AnzKwQMveCQXP1jVUvuaOReWdhGj
2024-12-04T09:20:18.136Z   UPJ3AnzKwQMveCQXP1jVUvuaOReWdhGj

![](Images/Results.JPG)
