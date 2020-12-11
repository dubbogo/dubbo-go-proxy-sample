# Dubbogo Proxy Examples

## What It Contains

* dubboproxy: A common example. Support POST to every single cluster, only defined one api.
* dubboquery: A url query to dubbo example. Url like `/xxx?a=a&b=b`. It's form format.
* dubbobody: A body query to dubbo example. Not read-only by params, but modify data.
* dubbouri: A uri query to dubbo example. Url like `/xxx/a/b`. It's rest format.
* httpquery: A uri query to http example. Url like `/xxx?a=a&b=b`. It's rest format.
* httpbody: A uri query to http example. Not read-only by params, but modify data.
* httpuri: A uri query to http example. Url like `/xxx/a/b`. It's rest format.
* mock: A uri query to mock result.

## How To Run

#### 1. Setup Zookeeper Server

#### 2. Prepare dubbbogoproxy

- Download proxy

```bash
git clone git@github.com:dubbogo/dubbo-go-proxy.git
```

- Compile

```bash
cd ${projectpath}/cmd/project
go build
```

- Move to run path

```bash
mv cmd ${targetpath}/
cd ${targetpath}
```

- Start

```bash
./proxy -c /${proxyPath}/sample/dubbogo/proxy/conf.yaml -a /${sampleProxyPath}/proxy/api_config.yaml 
```