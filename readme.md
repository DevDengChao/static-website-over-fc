# Static website over fc

This sample project shows how to deploy your static website onto Aliyun's Function compute.

### How to use?

Execute `fun-local-start.cmd` script or run `fun local start`, then your website is running inside Fc now.

Let's check it out at http://localhost:8000/2016-08-15/proxy/service/function

### How it works?

0. We deploy our static website to function compute's custom runtime environment.
0. We start a light-weight [http-server](https://www.npmjs.com/package/http-server) to host our content at port 9000 inside FC.
0. Fc forward outside's request to inner server, thus your content is showing.
