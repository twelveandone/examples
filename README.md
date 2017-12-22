# Examples

<a href="https://travis-ci.org/iris-contrib/examples"><img src="https://img.shields.io/travis/iris-contrib/examples.svg?branch=v8&style=flat-square" alt="Build Status"></a>
<a href="https://github.com/iris-contrib/examples/blob/v8/LICENSE"><img src="https://img.shields.io/badge/%20license-MIT%20%20License%20-E91E63.svg?style=flat-square" alt="License"></a>
<a href="https://github.com/kataras/iris/blob/v8/HISTORY.md"><img src="https://img.shields.io/badge/version-8.5.9-final%20-blue.svg?style=flat-square" alt="CHANGELOG/HISTORY"></a>

This repository provides easy to understand code snippets on how to get started with web development with the Go programming language using the [Iris v8](https://github.com/kataras/iris/tree/v8) web framework.

It doesn't contains "best ways" neither explains all its features. It's just a simple, practical cookbook for young Gophers!

## Table of Contents

* [Overview](overview)
    * [Hello world!](hello-world/main.go)
    * [Glimpse](overview/main.go)
    * [Tutorial: Online Visitors](tutorial/online-visitors/main.go)
    * [Tutorial: URL Shortener using BoltDB](tutorial/url-shortener/main.go)
    * [Tutorial: DropzoneJS + Go: How to build a file upload form](tutorial/dropzonejs/main.go)
    * [Tutorial:Iris Go Framework + MongoDB](https://medium.com/go-language/iris-go-framework-mongodb-552e349eab9c)
* [Structuring](structuring)
    * [Bootstrapper](structuring/bootstrap/bootstrap/bootstrapper.go)
    * [MVC with Repository and Service layer Overview](mvc/overview/main.go)
    * [Login (MVC with Single Responsibility package)](structuring/login-mvc-single-responsible-package/main.go)
    * [Login (MVC with Datamodels, Datasource, Repository and Service layer)](mvc/login/main.go)
* [HTTP Listening](http-listening)
    * [Common, with address](http-listening/listen-addr/main.go)
    * [UNIX socket file](http-listening/listen-unix/main.go)
    * [TLS](http-listening/listen-tls/main.go)
    * [Letsencrypt (Automatic Certifications)](http-listening/listen-letsencrypt/main.go)
    * [Custom net.Listener](http-listening/custom-listener/main.go)
    * [SO_REUSEPORT for unix systems](http-listening/custom-listener/unix-reuseport/main.go)
    * [Omit server errors](http-listening/listen-addr/omit-server-errors/main.go)
    * [Custom HTTP Server](http-listening/custom-httpserver/easy-way/main.go)
    * [Custom HTTP Server (STD)](http-listening/custom-httpserver/std-way/main.go)
    * [Multi HTTP Servers](http-listening/custom-httpserver/multi/main.go)
    * [Graceful Shutdown](http-listening/graceful-shutdown/default-notifier/main.go)
* [Configuration](configuration)
    * [Functional](configuration/functional/main.go)
    * [From Configuration Struct](configuration/from-configuration-structure/main.go)
    * [Import from YAML file](configuration/from-yaml-file/main.go)
        * [Share Configuration between multiple instances](configuration/from-yaml-file/shared-configuration/main.go)
    * [Import from TOML file](configuration/from-toml-file/main.go)
* [Routing](routing)
    * [Overview](routing/overview/main.go)
    * [Basic](routing/basic/main.go)
    * [Custom HTTP Errors](routing/http-errors/main.go)
    * [Dynamic Path](routing/dynamic-path/main.go)
    * [Root level wildcard path](routing/dynamic-path/root-wildcard/main.go)
    * [Reverse routing](routing/reverse/main.go)
    * [Custom wrapper](routing/custom-wrapper/main.go)
    * [Route State](routing/route-state/main.go)
* [MVC](mvc)
    * [Hello world](mvc/hello-world/main.go)
    * [Session Controller](mvc/session-controller/main.go)
    * [Overview - Plus Repository and Service layers](mvc/overview/main.go)
    * [Login showcase - Plus Repository and Service layers](mvc/login/main.go)
* [Custom Context](routing/custom-context)
    * [Method Overriding](routing/custom-context/method-overriding/main.go)
    * [New Implementation](routing/custom-context/new-implementation/main.go)
* [Convert http.Handler](convert-handlers)
    * [From func(http.ResponseWriter, *http.Request, http.HandlerFunc)](convert-handlers/negroni-like/main.go)
    * [From http.Handler or http.HandlerFunc](convert-handlers/nethttp/main.go)
* [Subdomains](subdomains)
    * [Single](subdomains/single/main.go)
    * [Multi](subdomains/multi/main.go)
    * [Wildcard](subdomains/wildcard/main.go)
    * [WWW](subdomains/www/main.go)
* [View](view)
    * [Overview](view/overview/main.go)
    * [Hi](view/template_html_0/main.go)
    * [A simple Layout](view/template_html_1/main.go)
    * [Layouts: `yield` and `render` tmpl funcs](view/template_html_2/main.go)
    * [The `urlpath` tmpl func](view/template_html_3/main.go)
    * [The `url` tmpl func](view/template_html_4/main.go)
    * [Inject Data Between Handlers](view/context-view-data/main.go)
    * [Embedding Templates Into App Executable File](view/embedding-templates-into-app/main.go)
* [Authentication](authentication)
    * [Basic Authentication](authentication/basicauth/main.go)
    * [OAUth2](authentication/oauth2/main.go)
    * [JWT](experimental-handlers/jwt/simple/main.go)
* [File Server](file-server)
    * [Favicon](file-server/favicon/main.go)
    * [Basic](file-server/basic/main.go)
    * [Embedding Files Into App Executable File](file-server/embedding-files-into-app/main.go)
    * [Send/Force-Download Files](file-server/send-files/main.go)
* [Single Page Applications](file-server/single-page-application)
    * [Single Page Application](file-server/single-page-application/basic/main.go)
    * [Embedded Single Page Application](file-server/single-page-application/embedded-single-page-application/main.go)
* [How to Read from *http.Request`](http_reqest)
    * [Bind JSON](http_request/read-json/main.go)
    * [Bind Form](http_request/read-form/main.go)
    * [Upload/Read Files](http_request/upload-files/main.go)
* [How to Write to http.ResponseWriter](http_responsewriter)
	* [Write `valyala/quicktemplate` templates](http_responsewriter/quicktemplate/main.go)
    * [Text, Markdown, HTML, JSON, JSONP, XML, Binary](http_responsewriter/write-rest/main.go)
    * [Stream Writer](http_responsewriter/stream-writer/main.go)
    * [Transactions](http_responsewriter/transactions/main.go)
* [Miscellaneous](miscellaneous)
    * [Request Logger](http_request/request-logger/main.go)
	* [Log Requests to a file](http_request/request-logger/request-logger-file/main.go)
    * [Localization and Internationalization](miscellaneous/i18n/main.go)
    * [Recovery](miscellaneous/recover/main.go)
    * [Profiling (pprof)](miscellaneous/pprof/main.go)
    * [Internal Application File Logger](miscellaneous/file-logger/main.go)
    * [Testing](testing/httptest/main_test.go)
    * [Caching](cache/simple/main.go)
    * [Yaag - API Automated Docs](apidoc/yaag/main.go)
* [Sessions](sessions)
    * [Overview](sessions/overview/main.go)
    * [Standalone](sessions/standalone/main.go)
    * [Secure Cookie](sessions/securecookie/main.go)
    * [Flash Messages](sessions/flash-messages/main.go)
    * [Database](sessions/database/main.go)
* [Websockets](websocket)
    * [Chat](websocket/chat/main.go)
    * [Native Messages](websocket/native-messages/main.go)
    * [Connection List](websocket/connectionlist/main.go)
    * [TLS Enabled](websocket/secure/main.go)
    * [Custom Raw Go Client](websocket/custom-go-client/main.go)
* [Experimental Handlers](experimental-handlers)
    * [Casbin wrapper](experimental-handlers/casbin/wrapper/main.go)
    * [Casbin middleware](experimental-handlers/casbin/middleware/main.go)
    * [Cloudwatch](experimental-handlers/cloudwatch/simple/main.go)
    * [CORS](experimental-handlers/cors/simple/main.go)
    * [JWT](experimental-handlers/jwt/main.go)
    * [Newrelic](experimental-handlers/newrelic/simple/main.go)
    * [Prometheus](experimental-handlers/prometheus/simple/main.go)
    * [Secure](experimental-handlers/secure/simple/main.go)
    * [Tollboothic](experimental-handlers/tollboothic/limit-handler/main.go)

> Do not forget to [star or watch the project](https://github.com/kataras/iris/stargazers) in order to stay updated with the latest tech trends!
> Examples are tested using Windows 10, Ubuntu 16.10 with [Microsoft's Visual Studio Code](https://code.visualstudio.com/) and built using the [Go 1.9](https://golang.org/dl).

## Run

1. Install Iris v8: https://github.com/kataras/iris/tree/v8#installation
2. clear yours previously `$GOPATH/src/github.com/iris-contrib/examples` folder or create new
3. download the Iris v8.5.9 (final): https://github.com/iris-contrib/examples/archive/v8.zip
4. extract the contents of the `examples-v8` folder that's inside the downloaded zip file to your `$GOPATH/src/github.com/iris-contrib/examples`
5. navigate to your `$GOPATH/src/github.com/iris-contrib/examples` folder if you're not already there and open a terminal/command prompt, execute the command: `go get ./...` and you're ready to GO:)

And run

```sh
$ cd $GOPATH/src/github.com/iris-contrib/examples/overview
$ go run main.go
```