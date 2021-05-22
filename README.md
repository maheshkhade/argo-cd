Docker commands to build the custom nginx webserver image:

```
#docker build --tag=automation-test .

#docker run --detach --publish=5001:80\
    --name=automation-test automation-test
```

Your static page should be accessible at http://localhost:5001/


##TODO##

- Create kubernetes cluster deployment with this custom image
- Make the webserver  accessible on http://automation-challange.cgi.com in the browser
- Add HTTPS only access
- Add TLS certificate
- CI/CD pipeline