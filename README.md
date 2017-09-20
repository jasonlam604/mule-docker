# Mule Runtime Dockerfile
Docker image for [Mule Runtime](https://docs.mulesoft.com/mule-user-guide/v/3.8/) by [MuleSoft](http://www.mulesoft.org)

## How to use
```
docker pull jasonlam604/mule
```

### Usage

For a simple application using 8181 port as HTTP

```
docker run -d -name mymule -p 8181:8181 -v ~/your-app-dir:/opt/mule/apps -v ~/your-log-dir:/opt/mule/logs jasonlam604/mule
```

#### Mount points

| Mount point       | Description                                                     |
|------------------ |-----------------------------------------------------------------|
|/opt/mule/apps     | Mule Application deployment directory                           |
|/opt/mule/domains  | Mule Domains deployment directory                               |
|/opt/mule/conf     | Configuration directory                                         |
|/opt/mule/logs     | Logs directory                                                  |

