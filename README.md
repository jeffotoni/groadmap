###### [Topics to be covered on our YouTube channel»](https://www.youtube.com/user/jeffotoni)

[Português](./README_ptbr.md)

> The intent of this guide is to give you an idea about the Go ecosystem and help guide your learning if you are confused. It is mainly focused on presenting the tools and concepts used in web development. Feel free to send comments
- suggestions or even a PR improving at some point. 

> I will be super happy to know that you would like to collaborate or that we helped in some way in your formation when it comes to Go.

# Go Roadmap

<img src="groadmap_new.png" alt="Roadmap Go" style="height: 98%; width:98%;"/>
<img src="groadmap.png" alt="Roadmap Go" style="height: 98%; width:98%;"/>

<object data="groadmap.pdf" type="application/pdf" width="80%" height="80%">
    <embed src="groadmap.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="groadmap.pdf">Download PDF</a>.</p>
    </embed>
</object>

# Sumary

## GO Basic & Intermediary

1. Basic & Intermediate Concepts 
        - [generics](https://gobootcamp.jeffotoni.com/en/pages/generics/introduction.html)  
        - [constants](https://gobootcamp.jeffotoni.com/en/pages/introduction/constants.html)  

    if/else, switch  
        - [switch](https://gobootcamp.jeffotoni.com/en/pages/structures_controlers/switch.html)  
        - [if / else](https://gobootcamp.jeffotoni.com/en/pages/structures_controlers/if-else.html)  

    Loops (for, range)  
        - [for](https://gobootcamp.jeffotoni.com/en/pages/structures_controlers/for-loop.html)  
        - [range](https://gobootcamp.jeffotoni.com/en/pages/structures_controlers/range.html)  

    Functions and Methods  
        - [functions](https://gobootcamp.jeffotoni.com/en/pages/functions/introduction.html)  
        - [variadic functions](https://gobootcamp.jeffotoni.com/en/pages/functions/variadic-functions.html)  
        - [return](https://gobootcamp.jeffotoni.com/en/pages/functions/return.html)  
        - [closures/anonymous functions](https://gobootcamp.jeffotoni.com/en/pages/functions/closures.html)  
        - [methods](https://gobootcamp.jeffotoni.com/en/pages/methods/function-comparison.html)  
        - [defer](https://gobootcamp.jeffotoni.com/en/pages/functions/defer.html)  

    Data Structures (array, slice, map, struct)  
        - [array](https://gobootcamp.jeffotoni.com/en/pages/arrays/introduction.html)  
        - [slice](https://gobootcamp.jeffotoni.com/en/pages/slices/introduction.html)  
        - [make](https://gobootcamp.jeffotoni.com/en/pages/slices/make.html)  
        - [new](https://gobootcamp.jeffotoni.com/en/pages/structs/new.html)  
        - [maps](https://gobootcamp.jeffotoni.com/en/pages/maps/introduction.html)  
        - [structs](https://gobootcamp.jeffotoni.com/en/pages/structs/introduction.html)  

    Pointers  
        - [pointers](https://gobootcamp.jeffotoni.com/en/pages/pointers/introduction.html)  

    Types  
        - [types](https://gobootcamp.jeffotoni.com/en/pages/types/types.html)  
        - [type interface](https://gobootcamp.jeffotoni.com/en/pages/types/types.html)  
        - [interface{}](https://gobootcamp.jeffotoni.com/en/pages/types/types-interface.html)  

    Initialization  
        - [iota](https://gobootcamp.jeffotoni.com/en/pages/introduction/iota.html)  
        - [func init](https://gobootcamp.jeffotoni.com/en/pages/introduction/init.html)  

    Errors, and Panic/Recover  
        - [error](https://gobootcamp.jeffotoni.com/en/pages/types/error.html)   
        - [panic](https://gobootcamp.jeffotoni.com/en/pages/erros/panic.html)  
        - [recover](https://gobootcamp.jeffotoni.com/en/pages/erros/recover.html)  
        

2. Goroutines  
    - [channel](https://gobootcamp.jeffotoni.com/en/pages/goroutines/channels.html)
    - [channel buffer](https://gobootcamp.jeffotoni.com/en/pages/goroutines/buffering.html)
    - [select](https://gobootcamp.jeffotoni.com/en/pages/goroutines/select.html)
    - [sync.Mutex](https://pkg.go.dev/sync#Mutex)
    - [sync.Map](https://pkg.go.dev/sync#Map)
    - [sync.WaitGroup](https://gobootcamp.jeffotoni.com/en/pages/goroutines/wait-groups.html)
    - [sync.Pool](https://pkg.go.dev/sync#Pool)

3. Runtime  
    - [runtime.GOMAXPROCS](https://pkg.go.dev/runtime#GOMAXPROCS)
    - [runtime.NumCPU()](https://pkg.go.dev/runtime#NumCPU)   
    - [runtime.NumGoroutine()](https://pkg.go.dev/runtime#NumGoroutine)
    
4. go  
    - [go test](https://gobootcamp.jeffotoni.com/en/pages/testes/introduction.html)
        - [go test -v]
        - [go test -run ^NameFunc$]
        - [go test -coverprofile](https://gobootcamp.jeffotoni.com/en/pages/testes/coverage.html)
        - [go test -bench . -benchmem](https://gobootcamp.jeffotoni.com/en/pages/testes/benchmark.html)
        - [go test -fuzz=Fuzz](https://gobootcamp.jeffotoni.com/en/pages/testes/fuzz.html)

    - go build & go run .
        - [go run .](https://gobootcamp.jeffotoni.com/en/pages/commands/go-run.html)
        - [go run -race .]
        - [CGO_ENABLED=0 go build]
        - [go build -ldflags="-s -w"]
        - [go build -gcflags '-m -l']
        - [GOOS=linux GOARCH=amd64 go build]
        - [go build GOARCH=wasm GOOS=js go build]
        - [go build -gcflags -S]
        - [go help buildmode]
        - [go build -buildmode=plugin]

    - [go install golang.org/x/website/tour@latest](https://pkg.go.dev/golang.org/x/tour)

5. Modules
    - package & import
        - [import ..](https://www.digitalocean.com/community/tutorials/importing-packages-in-go)
        - [import "fmt"](https://www.digitalocean.com/community/tutorials/importing-packages-in-go)
        - [import "my-pkg/util"](https://www.digitalocean.com/community/tutorials/importing-packages-in-go)
        - [package mypkg](https://www.digitalocean.com/community/tutorials/how-to-write-packages-in-go)

    - [go.mod](https://gobootcamp.jeffotoni.com/en/pages/commands/go-mod.html)
    - [go.sum](https://faun.pub/understanding-go-mod-and-go-sum-5fd7ec9bcc34)
    - [go mod init](https://gobootcamp.jeffotoni.com/en/pages/commands/go-mod.html)
    - [go mod tidy]
    - [go mod vendor]
    - [go mod download]
    - [go env](https://linuxcommandlibrary.com/man/go-env)
    - [GO111MODULE=on](https://www.codetd.com/pt/article/12986396)
    - [GOARCH=amd64](https://buaq.net/go-1925.html)
    - [GOPRIVATE](https://goproxy.io/docs/GOPRIVATE-env.html)
    - [GOPROXY](https://jfrog.com/blog/why-goproxy-matters-and-which-to-pick/)
    - [GOSUMDB](https://goproxy.io/docs/GOSUMDB-env.html)

6. Patterns
    - [Build](https://refactoring.guru/design-patterns/builder/go/example#example-0)
    - [Factory Method](https://refactoring.guru/design-patterns/factory-method/go/example#example-0)
    - [Abstract Factory](https://refactoring.guru/design-patterns/abstract-factory/go/example#example-0)
    - [Adapter](https://refactoring.guru/design-patterns/adapter/go/example#example-0)
    - [Bridge](https://refactoring.guru/design-patterns/bridge/go/example#example-0)
    - [Facade](https://refactoring.guru/design-patterns/facade/go/example#example-0)
    - [Composite](https://refactoring.guru/design-patterns/composite/go/example#example-0)
    - [Decorator](https://refactoring.guru/design-patterns/decorator/go/example#example-0)
    - [Prototype](https://refactoring.guru/design-patterns/prototype/go/example#example-0)
    - [Singleton](https://refactoring.guru/design-patterns/singleton/go/example#example-1)
    - [Template Method](https://refactoring.guru/design-patterns/template-method/go/example#example-0)

7. fasthttp
    - Frameworks
        - [Fiber](https://gobootcamp.jeffotoni.com/en/pages/fiber/introduction.html)
        - [Gramework](https://gobootcamp.jeffotoni.com/en/pages/rest/gramework.html)

    - Middleware
        - Iu
        - [fiber-middleware](https://gobootcamp.jeffotoni.com/en/pages/fiber/middlewares.html)

    - Routing
        - [fasthttp-routing](https://github.com/qiangxue/fasthttp-routing)
        - [atreugo](https://github.com/savsgio/atreugo)

    - Websocket
        - fast-http-socket
        - [fastws](https://github.com/dgrr/fastws)

8. net/http
    - Server
        - [http.NewServeMux](https://pkg.go.dev/net/http#NewServeMux)
        - [http.Server](https://gobootcamp.jeffotoni.com/en/pages/net_http_server/http-server.html)
        - [http.HandlerFunc](https://pkg.go.dev/net/http#HandlerFunc)
        - [http.Handle](https://pkg.go.dev/net/http#Handle)
        - [http.Handler](https://gobootcamp.jeffotoni.com/en/pages/net_http_server/http_handler.html)
        - [http.Status](https://pkg.go.dev/net/http#Status)
        - [next.ServeHTTP](https://gobootcamp.jeffotoni.com/en/pages/net_http_server/http-server.html)
        - [ListenAndServe](https://gobootcamp.jeffotoni.com/en/pages/net_http_server/listen-and-serve.html)
        - [ListenAndServeTLS](https://pkg.go.dev/net/http#ListenAndServeTLS)
        - [http.FileServer](https://gobootcamp.jeffotoni.com/en/pages/net_http_server/file-server.html)
        - [http.Dir](https://pkg.go.dev/net/http#Dir)
        - [http.StripPrefix](https://pkg.go.dev/net/http#StripPrefix)
        - Embed
        - [http.FS](https://pkg.go.dev/net/http#FS)
        - html/template
            - [template.ParseFiles](https://pkg.go.dev/html/template#ParseFiles)
            - [template.Parse](https://pkg.go.dev/html/template#Parse)
            - [template.ParseFS](https://pkg.go.dev/html/template#ParseFS)
            - [template.New](https://pkg.go.dev/html/template#New)
            - [template.Must](https://pkg.go.dev/html/template#Must)
            - [template.Execute](https://pkg.go.dev/html/template#Execute)
            - [template.ExecuteTemplate](https://pkg.go.dev/html/template#ExecuteTemplate)

    - Client
        - [http.Transport](https://pkg.go.dev/net/http#Transport)
        - [http.Client](https://gobootcamp.jeffotoni.com/en/pages/net_http_client/client.html)
        - [http.Get](https://gobootcamp.jeffotoni.com/en/pages/net_http_client/http-get.html)
        - [http.Post](https://gobootcamp.jeffotoni.com/en/pages/net_http_client/http-post.html)
        - [http.PostForm](https://pkg.go.dev/net/http#PostForm)
        - [ioutil.ReadAll(r io.Reader)](https://pkg.go.dev/io/ioutil#ReadAll)
        - [http.NewRequest](https://gobootcamp.jeffotoni.com/en/pages/net_http_client/http-new-request.html)
        - [http.NewRequestContext](https://pkg.go.dev/net/http#NewRequestContext)
        - [Context.WithCancel](https://pkg.go.dev/context#WithCancel)

    - Web Frameworks
        - [gin](https://gobootcamp.jeffotoni.com/en/pages/rest/gin.html)
        - [echo](https://gobootcamp.jeffotoni.com/en/pages/rest/echo.html)
        - [beego](https://gobootcamp.jeffotoni.com/en/pages/rest/beego.html)
        - [iris](https://github.com/kataras/iris)
        - [martini](https://github.com/go-martini/martini)
        - gocraft
        - [revel](https://github.com/revel/revel)
        - [buffalo](https://github.com/gobuffalo/buffalo)
        - [chi](https://gobootcamp.jeffotoni.com/en/pages/rest/chi.html)
        - [macaron](https://gobootcamp.jeffotoni.com/en/pages/rest/macaron.html)
        - [webgo](https://github.com/bnkamalesh/webgo)
        - [quick](https://github.com/jeffotoni/quick)

    - Routers
        - [alien](https://github.com/gernest/alien)
        - [bellt](https://github.com/GuilhermeCaruso/bellt)
        - [bone](https://github.com/go-zoo/bone)
        - [bxog](https://github.com/claygod/Bxog)
        - [goroute](https://github.com/cloudfoundry/gorouter)
        - [httprouter](https://github.com/julienschmidt/httprouter)
        - [httptreemux](https://github.com/dimfeld/httptreemux)
        - [gorilla/mux](https://gobootcamp.jeffotoni.com/en/pages/router/gorilla-mux.html)
        - [ozzo-routing](https://github.com/go-ozzo/ozzo-routing)
        - pure
        - [siesta](https://github.com/VividCortex/siesta)
        - [vestigo](https://github.com/husobee/vestigo)
        - [xmux](https://github.com/rs/xmux)
        - [xujiajun/gorouter](https://github.com/xujiajun/gorouter)

    - Middlewares
        - [negroni](https://github.com/urfave/negroni)
        - [muxchain](https://github.com/stephens2424/muxchain)
        - [go-wrap](https://github.com/hexdigest/gowrap)
        - [interpose](https://github.com/carbocation/interpose)
        - [rye](https://github.com/InVisionApp/rye)
        - Middeware libs
            - [CORS](https://docs.gofiber.io/api/middleware/cors)
            - [rate limit](https://mauricio.github.io/2021/12/30/rate-limiting-in-go.html)
            - [logging](https://gomanual.jeffotoni.com/pages/fiber/logger.html)
            - [metrics](https://prometheus.io/docs/guides/go-application/)
            - [auth](https://docs.gofiber.io/api/middleware/basicauth)
            - tracing
            - [limiter](https://docs.gofiber.io/api/middleware/limiter)
            - [jwt](https://github.com/gofiber/jwt)
            - [logger](https://gomanual.jeffotoni.com/pages/fiber/logger.html)
            - [cache](https://gomanual.jeffotoni.com/pages/fiber/cache.html)
            - Instrumentation
                - [Prometheus](https://github.com/prometheus/prometheus)
                - [Datadog](https://github.com/DataDog/datadog-agent)
                - [New Relic](https://github.com/newrelic/go-agent)
                - [loggly](https://github.com/segmentio/go-loggly)

9. Previous Knowledge
    - [git](https://git-scm.com/)
        - [git init](http://guides.beanstalkapp.com/version-control/common-git-commands.html#git-init)
        - [git add .](http://guides.beanstalkapp.com/version-control/common-git-commands.html#git-add)
        - [git commit](http://guides.beanstalkapp.com/version-control/common-git-commands.html#git-commit)
        - [git push](http://guides.beanstalkapp.com/version-control/common-git-commands.html#git-push)
        - [git merge](http://guides.beanstalkapp.com/version-control/common-git-commands.html#git-merge)
        - [git rebase](https://git-scm.com/book/pt-br/v2/Branches-no-Git-Rebase)
        - [git log](http://guides.beanstalkapp.com/version-control/common-git-commands.html#git-log)
        - [git diff](https://git-scm.com/docs/git-diff)
        - [git show](https://git-scm.com/docs/git-show)
        - [git clone](http://guides.beanstalkapp.com/version-control/common-git-commands.html#git-clone)

    - [docker](https://www.docker.com/)
        - [docker run](https://docs.docker.com/engine/reference/commandline/run/)
        - [docker build](https://docs.docker.com/engine/reference/commandline/build/)
        - [docker images](https://docs.docker.com/engine/reference/commandline/images/)
        - [docker push](https://docs.docker.com/engine/reference/commandline/push/)
        - [docker login](https://docs.docker.com/engine/reference/commandline/login/)
        - [docker ps -a](https://docs.docker.com/engine/reference/commandline/ps/)

    - [docker-compose](https://docs.docker.com/compose/)
    - [sql basic syntax](https://www.w3schools.com/sql/sql_syntax.asp)
    - [openssl](https://www.openssl.org/)
    - [ssh-keygen](https://en.wikipedia.org/wiki/Ssh-keygen)
    - [https/http](https://en.wikipedia.org/wiki/Hyper_Text_Transfer_Protocol_Secure)
    - [tls/mtls](https://www.cloudflare.com/learning/access-management/what-is-mutual-tls/)

    - Relational
        - [PostgreSQL](https://www.postgresql.org/)
        - [MySql](https://www.mysql.com/)
        - [SqlServer](https://www.microsoft.com/sql-server/sql-server-2019)
        - [Oracle](https://www.oracle.com/br/database/)
        - [MariaDB](https://mariadb.org/)

    - NoSql
        - [MongoDB](https://www.mongodb.com)
        - [Cassandra](https://cassandra.apache.org/_/index.html)
        - [RavenDB](https://ravendb.net/)
        - [RethinkDB](https://rethinkdb.com/)
        - [CouchDB](https://couchdb.apache.org/)
        - [CockroachDB](https://www.cockroachlabs.com/)
        - [Redis](https://redis.io/)
        - [Elasticsearch](https://www.elastic.co/what-is/elasticsearch)
        - [ArangoDB](https://www.arangodb.com/)

    - Queue
        - [RabbitMQ](https://www.rabbitmq.com/)
        - [KubeMQ](https://kubemq.io/)
        - [SQS Aws](https://aws.amazon.com/sqs/)
        - [Pub/Sub Google Cloud](https://cloud.google.com/pubsub)
        - [Beanstalk](https://aws.amazon.com/elasticbeanstalk/)
        - [ActiveMQ](https://activemq.apache.org/)

    - Stream
        - [Kafka](https://kafka.apache.org/)
        - [Redpanda](https://redpanda.com/)
        - [KubeMQ](https://kubemq.io/)
        - [Nats](https://nats.io/)
        - [Kinesis Aws](https://aws.amazon.com/kinesis/)

    - Protocols
        - Applications
            - [gRPC](https://grpc.io/)
            - [rpc](https://en.wikipedia.org/wiki/Remote_procedure_call)
            - [xml-rpc](https://en.wikipedia.org/wiki/XML-RPC)
            - [WebSocket](https://developer.mozilla.org/docs/Web/API/WebSockets_API)
        - Serialization
            - [Protobuf Buffer](https://developers.google.com/protocol-buffers)
            - [gob](https://go.dev/blog/gob)
            - [msgpack](https://msgpack.org/)
            - [bson](https://www.mongodb.com/docs/manual/reference/bson-types/)
            - [Avro](https://avro.apache.org/)
            - [Thrift](https://thrift.apache.org/)
            - [json](https://www.json.org/json-en.html)
            - [xml](https://pt.wikipedia.org/wiki/XML)
        - [tcp](https://en.wikipedia.org/wiki/Transmission_Control_Protocol)
        - [udp](https://en.wikipedia.org/wiki/User_Datagram_Protocol)
        - [http](https://developer.mozilla.org/docs/Web/HTTP/Overview)
        - [http2](https://developers.google.com/web/fundamentals/performance/http2)
        - [http3](https://en.wikipedia.org/wiki/HTTP/3)
        - [MQTT](https://mqtt.org/)
