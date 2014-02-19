Mono
==========

Base Mono 3.2.6 container for octohost.

To use an already built container:

`docker pull octohost/mono`

Or you can build it from this source:

`docker build -t your-organization/mono`

Once it's built, you can use it in your web project Dockerfile:

```
FROM octohost/mono

ADD app/ .
EXPOSE 5000
CMD ["/opt/mono/bin/mono", "PutYourAppHere.exe", "5000"]
```

Completely stolen from: [http://friism.com/running-net-apps-on-docker](http://friism.com/running-net-apps-on-docker).