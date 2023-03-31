##### [Temas a serem abordados em nosso canal do YouTube»](https://www.youtube.com/user/jeffotoni)

[English](./README.md)

> A intenção deste guia é dar uma ideia sobre o ecossistema Go e ajudar a orientar seu aprendizado se você estiver confuso. Ele é focado principalmente em apresentar as ferramentas e conceitos ultilizados no desenvolvimento web.

# Go Roadmap

<img src="groadmap.png" alt="Roadmap Go" style="height: 90%; width:90%;"/>

<object data="groadmap.pdf" type="application/pdf" width="80%" height="80%">
    <embed src="groadmap.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="groadmap.pdf">Download PDF</a>.</p>
    </embed>
</object>

# Sumary

## GO Básico e Intermediário  

1. Conceitos Básicos e Intermediários  

    Variáveis, Tipos e Operadores    
        - [genéricos](https://gobootcamp.jeffotoni.com/br/pages/generics/introduction.html)     
        - [constantes](https://gobootcamp.jeffotoni.com/br/pages/introduction/constants.html)    

    if/else, switch    
        - [switch](https://gobootcamp.jeffotoni.com/br/pages/structures_controlers/switch.html)    
        - [if/else](https://gobootcamp.jeffotoni.com/br/pages/structures_controlers/if-else.html)    

    Loops (for, range)    
        - [for](https://gobootcamp.jeffotoni.com/br/pages/structures_controlers/for-loop.html)    
        - [range](https://gobootcamp.jeffotoni.com/br/pages/structures_controlers/range.html)    

    Funções e Métodos    
        - [funções](https://gobootcamp.jeffotoni.com/br/pages/functions/introduction.html)    
        - [funções variádicas](https://gobootcamp.jeffotoni.com/br/pages/functions/variadic-functions.html)    
        - [return](https://gobootcamp.jeffotoni.com/br/pages/functions/return.html)    
        - [closures/funções anônimas](https://gobootcamp.jeffotoni.com/br/pages/functions/closures.html)    
        - [métodos](https://gobootcamp.jeffotoni.com/br/pages/methods/function-comparison.html)    
        - [defer](https://gobootcamp.jeffotoni.com/br/pages/functions/defer.html)    

    Estruturas de Dados (array, slice, map, struct)    
        - [array](https://gobootcamp.jeffotoni.com/br/pages/arrays/introduction.html)    
        - [slice](https://gobootcamp.jeffotoni.com/br/pages/slices/introduction.html)    
        - [make](https://gobootcamp.jeffotoni.com/br/pages/slices/make.html)    
        - [new](https://gobootcamp.jeffotoni.com/br/pages/structs/new.html)    
        - [maps](https://gobootcamp.jeffotoni.com/br/pages/maps/introduction.html)    
        - [structs](https://gobootcamp.jeffotoni.com/br/pages/structs/introduction.html)    

    Ponteiros    
        - [ponteiros](https://gobootcamp.jeffotoni.com/br/pages/pointers/introduction.html)    

    Tipos    
        - [tipos](https://gobootcamp.jeffotoni.com/br/pages/types/types.html)    
        - [interface de tipo](https://gobootcamp.jeffotoni.com/br/pages/types/types.html)    
        - [interface{}](https://gobootcamp.jeffotoni.com/br/pages/types/types-interface.html)    

    Inicialização    
        - [iota](https://gobootcamp.jeffotoni.com/br/pages/introduction/iota.html)    
        - [func init](https://gobootcamp.jeffotoni.com/br/pages/introduction/init.html)    

    Erros e Panic/Recover    
        - [erro](https://gobootcamp.jeffotoni.com/br/pages/types/error.html)     
        - [panic](https://gobootcamp.jeffotoni.com/br/pages/erros/panic.html)    
        - [recover](https://gobootcamp.jeffotoni.com/br/pages/erros/recover.html)

## Goroutines em Go  

2. Goroutine  
        - [canal](https://gobootcamp.jeffotoni.com/br/pages/goroutines/channels.html)  
        - [buffer de canal](https://gobootcamp.jeffotoni.com/br/pages/goroutines/buffering.html)  
        - [select](https://gobootcamp.jeffotoni.com/br/pages/goroutines/select.html)  
        - [sync.Mutex](https://golang.org/pkg/sync/#Mutex)  
        - [sync.Map](https://golang.org/pkg/sync/#Map)  
        - [sync.WaitGroup](https://gobootcamp.jeffotoni.com/br/pages/goroutines/wait-groups.html)  
        - [sync.Pool](https://golang.org/pkg/sync/#Pool)  

## Runtime  

3. Runtime   
        - [runtime.GOMAXPROCS](https://golang.org/pkg/runtime/#GOMAXPROCS)  
        - [runtime.NumCPU()](https://golang.org/pkg/runtime/#NumCPU)     
        - [runtime.NumGoroutine()](https://golang.org/pkg/runtime/#NumGoroutine)  

## Go  

4. 
    Go Test  
        - [go test](https://gobootcamp.jeffotoni.com/br/pages/testes/introduction.html)  
        - [go test -bench . -benchmem](https://gobootcamp.jeffotoni.com/br/pages/testes/benchmark.html)  
        - [go test -coverprofile](https://gobootcamp.jeffotoni.com/br/pages/testes/coverage.html)  
        - [go test -fuzz=Fuzz](https://gobootcamp.jeffotoni.com/br/pages/testes/fuzz.html)  
        - [go test -run ^NameFunc$]  
        - [go test -v]  

    Go Build & Go Run  
        - [CGO_ENABLED=0 go build]  
        - [go build -buildmode=plugin]  
        - [go build -gcflags -S]  
        - [go build -gcflags '-m -l']  
        - [go build -ldflags="-s -w"]  
        - [GOOS=linux GOARCH=amd64 go build]  
        - [go build GOARCH=wasm GOOS=js go build]  
        - [go help buildmode]  
        - [go run .](https://gobootcamp.jeffotoni.com/br/pages/commands/go-run.html)  
        - [go run -race .]  

    Instalação  
        - [go install golang.org/x/website/tour@latest](https://pkg.go.dev/golang.org/x/tour)  

## Modules  

5. Pacote e Importação  
        - [importação](https://golang.org/doc/code.html#ImportingPackages)  
        - [import "fmt"](https://golang.org/pkg/fmt/)  
        - [import "meu-pacote/util"](https://golang.org/doc/code.html#ImportingPackages)  
        - [pacote meu-pacote](https://golang.org/doc/code.html#Packages)  

    Recursos do Go Module  
        - [go.mod](https://golang.org/cmd/go/#hdr-The_go_mod_file)  
        - [go.sum](https://golang.org/ref/mod#go-sum-files)  
        - [go mod init](https://gobootcamp.jeffotoni.com/br/pages/commands/go-mod.html)  
        - [go mod tidy]  
        - [go mod vendor]  
        - [go mod download]  
        - [go env](https://linuxcommandlibrary.com/man/go-env)  
        - [GO111MODULE=on](https://www.codetd.com/pt/article/12986396)  
        - [GOARCH=amd64](https://buaq.net/go-1925.html)  
        - [GOPRIVATE](https://goproxy.io/docs/GOPRIVATE-env.html)  
        - [GOPROXY](https://jfrog.com/blog/why-goproxy-matters-and-which-to-pick/)  
        - [GOSUMDB](https://goproxy.io/docs/GOSUMDB-env.html) 

## Pattern   

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

## Fasthttp  

7. 
    Frameworks
        - [Fiber](https://gobootcamp.jeffotoni.com/br/pages/fiber/introduction.html)  
        - [Gramework](https://gobootcamp.jeffotoni.com/br/pages/rest/gramework.html)  

    Middleware  
        - Iu  
        - [fiber-middleware](https://gobootcamp.jeffotoni.com/br/pages/fiber/middlewares.html)  

    Routing  
        - [fasthttp-routing](https://github.com/qiangxue/fasthttp-routing)  
        - [atreugo](https://github.com/savsgio/atreugo)  

    Websocket  
        - fast-http-socket  
        - [fastws](https://github.com/dgrr/fastws)  

## Net/Http  

8.   
    
    Server  
        - [http.NewServeMux](https://pkg.go.dev/net/http#NewServeMux)  
        - [http.Server](https://gobootcamp.jeffotoni.com/br/pages/net_http_server/http-server.html)  
        - [http.HandlerFunc](https://pkg.go.dev/net/http#HandlerFunc)  
        - [http.Handle](https://pkg.go.dev/net/http#Handle)  
        - [http.Handler](https://gobootcamp.jeffotoni.com/br/pages/net_http_server/http_handler.html)  
        - [http.Status](https://pkg.go.dev/net/http#Status)  
        - [next.ServeHTTP](https://gobootcamp.jeffotoni.com/br/pages/net_http_server/http-server.html)  
        - [ListenAndServe](https://gobootcamp.jeffotoni.com/br/pages/net_http_server/listen-and-serve.html)  
        - [ListenAndServeTLS](https://pkg.go.dev/net/http#ListenAndServeTLS)  
        - [http.FileServer](https://gobootcamp.jeffotoni.com/br/pages/net_http_server/file-server.html)  
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

    Cliente  
        - [http.Transport](https://pkg.go.dev/net/http#Transport)  
        - [http.Client](https://gobootcamp.jeffotoni.com/br/pages/net_http_client/client.html)  
        - [http.Get](https://gobootcamp.jeffotoni.com/br/pages/net_http_client/http-get.html)  
        - [http.Post](https://gobootcamp.jeffotoni.com/br/pages/net_http_client/http-post.html)  
        - [http.PostForm](https://pkg.go.dev/net/http#PostForm)  
        - [ioutil.ReadAll(r io.Reader)](https://pkg.go.dev/io/ioutil#ReadAll)  
        - [http.NewRequest](https://gobootcamp.jeffotoni.com/br/pages/net_http_client/http-new-request.html)  
        - [http.NewRequestContext](https://pkg.go.dev/net/http#NewRequestContext)  
        - [Context.WithCancel](https://pkg.go.dev/context#WithCancel)  

    Frameworks Web    
        - [gin](https://gobootcamp.jeffotoni.com/br/pages/rest/gin.html)  
        - [echo](https://gobootcamp.jeffotoni.com/br/pages/rest/echo.html)  
        - [beego](https://gobootcamp.jeffotoni.com/br/pages/rest/beego.html)  
        - [iris](https://github.com/kataras/iris)  
        - [martini](https://github.com/go-martini/martini)  
        - gocraft  
        - [revel](https://github.com/revel/revel)  
        - [buffalo](https://github.com/gobuffalo/buffalo)  
        - [chi](https://gobootcamp.jeffotoni.com/br/pages/rest/chi.html)  
        - [macaron](https://gobootcamp.jeffotoni.com/br/pages/rest/macaron.html)  
        - [webgo](https://github.com/bnkamalesh/webgo)  
        - [quick](https://github.com/jeffotoni/quick)  

    Roteadores  
        - [alien](https://github.com/gernest/alien)  
        - [bellt](https://github.com/GuilhermeCaruso/bellt)  
        - [bone](https://github.com/go-zoo/bone)  
        - [bxog](https://github.com/claygod/Bxog)  
        - [goroute](https://github.com/cloudfoundry/gorouter)  
        - [httprouter](https://github.com/julienschmidt/httprouter)  
        - [httptreemux](https://github.com/dimfeld/httptreemux)  
        - [gorilla/mux](https://gobootcamp.jeffotoni.com/br/pages/router/gorilla-mux.html)  
        - [ozzo-routing](https://github.com/go-ozzo/ozzo-routing)  
        - pure  
        - [siesta](https://github.com/VividCortex/siesta)  
        - [vestigo](https://github.com/husobee/vestigo)  
        - [xmux](https://github.com/rs/xmux)  
        - [xujiajun/gorouter](https://github.com/xujiajun/gorouter)  

    Middlewares  
        - [negroni](https://github.com/urfave/negroni)  
        - [muxchain](https://github.com/stephens2424/muxchain)  
        - [go-wrap](https://github.com/hexdigest/gowrap)  
        - [interpose](https://github.com/carbocation/interpose)  
        - [rye](https://github.com/InVisionApp/rye)  

    Middeware Libs  
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


## Previous Knowledge  

9.    
    Git  
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
    

    [Docker](https://www.docker.com/)  
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

    Relational  
        - [PostgreSQL](https://www.postgresql.org/)  
        - [MySql](https://www.mysql.com/)  
        - [SqlServer](https://www.microsoft.com/sql-server/sql-server-2019)  
        - [Oracle](https://www.oracle.com/br/database/)  
        - [MariaDB](https://mariadb.org/)  
 
    NoSql  
        - [MongoDB](https://www.mongodb.com)  
        - [Cassandra](https://cassandra.apache.org/_/index.html)  
        - [RavenDB](https://ravendb.net/)  
        - [RethinkDB](https://rethinkdb.com/)  
        - [CouchDB](https://couchdb.apache.org/)  
        - [CockroachDB](https://www.cockroachlabs.com/)  
        - [Redis](https://redis.io/)  
        - [Elasticsearch](https://www.elastic.co/what-is/elasticsearch)  
        - [ArangoDB](https://www.arangodb.com/)  

    Queue  
        - [RabbitMQ](https://www.rabbitmq.com/)  
        - [KubeMQ](https://kubemq.io/)  
        - [SQS Aws](https://aws.amazon.com/sqs/)  
        - [Pub/Sub Google Cloud](https://cloud.google.com/pubsub)  
        - [Beanstalk](https://aws.amazon.com/elasticbeanstalk/)  
        - [ActiveMQ](https://activemq.apache.org/)  

    Stream  
        - [Kafka](https://kafka.apache.org/)  
        - [Redpanda](https://redpanda.com/)  
        - [KubeMQ](https://kubemq.io/)  
        - [Nats](https://nats.io/)  
        - [Kinesis Aws](https://aws.amazon.com/kinesis/)  

    Protocols  
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
