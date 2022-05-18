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

# Sumário

1. Conceitos Básicos & Intermediários
    - [generics](https://gomanual.jeffotoni.com/pages/generics/) 
    - [constantes](https://gomanual.jeffotoni.com/pages/language_introduction/introduction/constants.html)
    - [variáveis](https://gomanual.jeffotoni.com/pages/language_introduction/introduction/variables.html)
    - [iota](https://gomanual.jeffotoni.com/pages/language_introduction/introduction/iota.html)
    - [func init](https://gomanual.jeffotoni.com/pages/language_introduction/introduction/init.html)
    - [types](https://gomanual.jeffotoni.com/pages/language_introduction/types/index.html)
    - [funcs](https://gomanual.jeffotoni.com/pages/functions/index.html)
    - [variadic](https://gomanual.jeffotoni.com/pages/functions/variadic_functions.html)
    - [return multiplos valores](https://gomanual.jeffotoni.com/pages/functions/return.html)
    - [closures / funções anônimas](https://gomanual.jeffotoni.com/pages/functions/closures.html)
    - [array](https://gomanual.jeffotoni.com/pages/arrays/index.html)
    - [slice](https://gomanual.jeffotoni.com/pages/slices/index.html)
    - [for](https://gomanual.jeffotoni.com/pages/structures_controlers/for.html)
    - [switch](https://gomanual.jeffotoni.com/pages/structures_controlers/switch.html)
    - [if / else](https://gomanual.jeffotoni.com/pages/structures_controlers/if_else.html)
    - [range](https://gomanual.jeffotoni.com/pages/structures_controlers/range.html)
    - [make](https://gomanual.jeffotoni.com/pages/slices/make.html)
    - [new](https://gomanual.jeffotoni.com/pages/structs/new.html)
    - [maps](https://gomanual.jeffotoni.com/pages/maps/index.html)
    - [ponteiros](https://gomanual.jeffotoni.com/pages/pointers/index.html)
    - [structs](https://gomanual.jeffotoni.com/pages/structs/index.html)
    - [métodos](https://gomanual.jeffotoni.com/pages/methods/index.html)
    - [type interface](https://gomanual.jeffotoni.com/pages/language_introduction/types/interface.html)
    - [interface{}](https://gomanual.jeffotoni.com/pages/language_introduction/types/interface_type.html)
    - [defer](https://gomanual.jeffotoni.com/pages/functions/defer.html)
    - [error](https://gomanual.jeffotoni.com/pages/language_introduction/types/error.html)
    - [panic](https://gomanual.jeffotoni.com/pages/erros/panic.html)
    - [recover](https://gomanual.jeffotoni.com/pages/erros/recover.html)

2. Goroutines
    - [channel](https://gomanual.jeffotoni.com/pages/goroutines/channels.html)
    - [channel buffer](https://gomanual.jeffotoni.com/pages/goroutines/channel_buffering.html)
    - [select](https://gomanual.jeffotoni.com/pages/goroutines/select.html)
    - [sync.Mutex](https://pkg.go.dev/sync#Mutex)
    - [sync.Map](https://pkg.go.dev/sync#Map)
    - [sync.WaitGroup](https://gomanual.jeffotoni.com/pages/goroutines/wait_groups.html)
    - [sync.Pool](https://pkg.go.dev/sync#Pool)

3. Runtime
    - [runtime.GOMAXPROCS](https://pkg.go.dev/runtime#GOMAXPROCS)
    - [runtime.NumCPU()](https://pkg.go.dev/runtime#NumCPU)   
    - [runtime.NumGoroutine()](https://pkg.go.dev/runtime#NumGoroutine)
    
4. go
    - [go test](https://gomanual.jeffotoni.com/pages/testes/index.html)
        - [go test -v](https://gomanual.jeffotoni.com/pages/testes/unit.html)
        - [go test -run ^NameFunc$](https://gomanual.jeffotoni.com/pages/testes/index.html)
        - [go test -coverprofile](https://gomanual.jeffotoni.com/pages/testes/coverage.html)
        - [go test ../../](https://gomanual.jeffotoni.com/pages/testes/index.html)
        - [go test -bench . -benchmem](https://gomanual.jeffotoni.com/pages/testes/benchmark.html)
        - [go test -fuzz=Fuzz](https://gomanual.jeffotoni.com/pages/testes/fuzz.html)

    - go build & go run .
        - [go run .](https://gomanual.jeffotoni.com/pages/commands/go_run.html)
        - [go run -race .](https://gomanual.jeffotoni.com/pages/commands/go_run.html)
        - [CGO_ENABLED=0 go build](https://gomanual.jeffotoni.com/pages/commands/go_build.html)
        - [go build -ldflags="-s -w"](https://gomanual.jeffotoni.com/pages/commands/go_build.html)
        - [go build -gcflags '-m -l'](https://gomanual.jeffotoni.com/pages/commands/go_build.html)
        - [GOOS=linux GOARCH=amd64 go build](https://gomanual.jeffotoni.com/pages/commands/go_build.html)
        - [go build GOARCH=wasm GOOS=js go build](https://gomanual.jeffotoni.com/pages/commands/go_build.html)
        - [go build -gcflags -S](https://gomanual.jeffotoni.com/pages/commands/go_build.html)
        - [go help buildmode](https://gomanual.jeffotoni.com/pages/commands/index.html)
        - [go build -buildmode=plugin](https://gomanual.jeffotoni.com/pages/commands/go_build.html)

    - [go install golang.org/x/website/tour@latest](https://gomanual.jeffotoni.com/pages/commands/go_install.html)

5. Modulos
    - package & import
        - [import ..](https://www.digitalocean.com/community/tutorials/importing-packages-in-go-pt)
        - [import "fmt"](https://www.digitalocean.com/community/tutorials/importing-packages-in-go-pt)
        - [import "my-pkg/util"](https://www.digitalocean.com/community/tutorials/importing-packages-in-go-pt)
        - [package mypkg](https://www.digitalocean.com/community/tutorials/how-to-write-packages-in-go-pt)

    - [go.mod](https://gomanual.jeffotoni.com/pages/commands/go_mod.html)
    - [go.sum](https://faun.pub/understanding-go-mod-and-go-sum-5fd7ec9bcc34)
    - [go mod init](https://gomanual.jeffotoni.com/pages/commands/go_mod.html)
    - [go mod tidy](https://gomanual.jeffotoni.com/pages/commands/go_mod.html)
    - [go mod vendor](https://gomanual.jeffotoni.com/pages/commands/go_mod.html)
    - [go mod download](https://gomanual.jeffotoni.com/pages/commands/go_mod.html)
    - [go env](https://linuxcommandlibrary.com/man/go-env)
    - [GO111MODULE=on](https://www.codetd.com/pt/article/12986396)
    - [GOARCH=amd64](https://buaq.net/go-1925.html)
    - [GOPRIVATE](https://goproxy.io/docs/GOPRIVATE-env.html)
    - [GOPROXY](https://jfrog.com/blog/why-goproxy-matters-and-which-to-pick/)
    - [GOSUMDB](https://goproxy.io/docs/GOSUMDB-env.html)

6. Patterns
    - [Build](https://refactoring.guru/pt-br/design-patterns/builder/go/example#example-0)
    - [Factory Method](https://refactoring.guru/pt-br/design-patterns/factory-method/go/example#example-0)
    - [Abstract Factory](https://refactoring.guru/pt-br/design-patterns/abstract-factory/go/example#example-0)
    - [Adapter](https://refactoring.guru/pt-br/design-patterns/adapter/go/example#example-0)
    - [Bridge](https://refactoring.guru/pt-br/design-patterns/bridge/go/example#example-0)
    - [Facade](https://refactoring.guru/pt-br/design-patterns/facade/go/example#example-0)
    - [Composite](https://refactoring.guru/pt-br/design-patterns/composite/go/example#example-0)
    - [Decorator](https://refactoring.guru/pt-br/design-patterns/decorator/go/example#example-0)
    - [Prototype](https://refactoring.guru/pt-br/design-patterns/prototype/go/example#example-0)
    - [Singleton](https://refactoring.guru/pt-br/design-patterns/singleton/go/example#example-1)
    - [Template Method](https://refactoring.guru/pt-br/design-patterns/template-method/go/example#example-0)

7. fasthttp
    - Frameworks
        - [Fiber](https://github.com/gofiber/fiber)
        - [Gramework](https://github.com/gramework/gramework)

    - Middleware
        - Iu
        - fiber-middleware

    - Routing
        - [fasthttp-routing](https://github.com/qiangxue/fasthttp-routing)
        - [atreugo](https://github.com/savsgio/atreugo)

    - Websocket
        - fast-http-socket
        - [fastws](https://github.com/dgrr/fastws)

8. net/http
    - Server
        - [http.NewServeMux](https://pkg.go.dev/net/http#NewServeMux)
        - [http.Server](https://pkg.go.dev/net/http#Server)
        - [http.HandlerFunc](https://pkg.go.dev/net/http#HandlerFunc)
        - [http.HandleFunc](https://pkg.go.dev/net/http#HandleFunc)
        - [http.Handle](https://pkg.go.dev/net/http#Handle)
        - [http.Handler](https://pkg.go.dev/net/http#Handler)
        - [http.Status](https://pkg.go.dev/net/http#Status)
        - [next.ServeHTTP](https://pkg.go.dev/net/http#ServeHTTP)
        - [ListenAndServe](https://pkg.go.dev/net/http#ListenAndServe)
        - [ListenAndServeTLS](https://pkg.go.dev/net/http#ListenAndServeTLS)
        - [http.FileServer](https://pkg.go.dev/net/http#FileServer)
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
        - [http.Client](https://pkg.go.dev/net/http#Client)
        - [http.Get](https://pkg.go.dev/net/http#Get)
        - [http.Post](https://pkg.go.dev/net/http#Post)
        - [http.PostForm](https://pkg.go.dev/net/http#PostForm)
        - [ioutil.ReadAll(r io.Reader)](https://pkg.go.dev/io/ioutil#ReadAll)
        - [http.NewRequest](https://pkg.go.dev/net/http#NewRequest)
        - [http.NewRequestContext](https://pkg.go.dev/net/http#NewRequestContext)
        - [Context.WithCancel](https://pkg.go.dev/context#WithCancel)

    - Frameworks Web
        - [gin](https://github.com/gin-gonic/gin)
        - [echo](https://github.com/labstack/echo)
        - [beego](https://github.com/beego/beego)
        - [iris](https://github.com/kataras/iris)
        - [martini](https://github.com/go-martini/martini)
        - gocraft
        - [revel](https://github.com/revel/revel)
        - [buffalo](https://github.com/gobuffalo/buffalo)
        - [chi](https://github.com/go-chi/chi)
        - [macaron](https://github.com/go-macaron/macaron)
        - [webgo](https://github.com/bnkamalesh/webgo)

    - Routers
        - [alien](https://github.com/gernest/alien)
        - [bellt](https://github.com/GuilhermeCaruso/bellt)
        - [bone](https://github.com/go-zoo/bone)
        - [bxog](https://github.com/claygod/Bxog)
        - [goroute](https://github.com/cloudfoundry/gorouter)
        - [httprouter](https://github.com/julienschmidt/httprouter)
        - [httptreemux](https://github.com/dimfeld/httptreemux)
        - [gorilla/mux](https://github.com/gorilla/mux)
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
        - Libs middleware
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
            - Instrumentação
                - [Prometheus](https://github.com/prometheus/prometheus)
                - [Datadog](https://github.com/DataDog/datadog-agent)
                - [New Relic](https://github.com/newrelic/go-agent)
                - [loggly](https://github.com/segmentio/go-loggly)

9. Conhecimentos Prévios
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
    - [https/http](https://pt.wikipedia.org/wiki/Hyper_Text_Transfer_Protocol_Secure)
    - [tls/mtls](https://www.cloudflare.com/pt-br/learning/access-management/what-is-mutual-tls/)

    - Relacional
        - [PostgreSQL](https://www.postgresql.org/)
        - [MySql](https://www.mysql.com/)
        - [SqlServer](https://www.microsoft.com/pt-br/sql-server/sql-server-2019)
        - [Oracle](https://www.oracle.com/br/database/)
        - [MariaDB](https://mariadb.org/)

    - NoSql
        - [MongoDB](https://www.mongodb.com/pt-br)
        - [Cassandra](https://cassandra.apache.org/_/index.html)
        - [RavenDB](https://ravendb.net/)
        - [RethinkDB](https://rethinkdb.com/)
        - [CouchDB](https://couchdb.apache.org/)
        - [CockroachDB](https://www.cockroachlabs.com/)
        - [Redis](https://redis.io/)
        - [Elasticsearch](https://www.elastic.co/pt/what-is/elasticsearch)
        - [ArangoDB](https://www.arangodb.com/)

    - Queue
        - [RabbitMQ](https://www.rabbitmq.com/)
        - [KubeMQ](https://kubemq.io/)
        - [SQS Aws](https://aws.amazon.com/pt/sqs/)
        - [Pub/Sub Google Cloud](https://cloud.google.com/pubsub?hl=pt-br)
        - [Beanstalk](https://aws.amazon.com/pt/elasticbeanstalk/)
        - [ActiveMQ](https://activemq.apache.org/)

    - Stream
        - [Kafka](https://kafka.apache.org/)
        - [Redpanda](https://redpanda.com/)
        - [KubeMQ](https://kubemq.io/)
        - [Nats](https://nats.io/)
        - [Kinesis Aws](https://aws.amazon.com/pt/kinesis/)

    - Protocolos
        - Aplicações
            - [gRPC](https://grpc.io/)
            - [rpc](https://pt.wikipedia.org/wiki/Chamada_de_procedimento_remoto)
            - [xml-rpc](https://pt.wikipedia.org/wiki/XML-RPC)
            - [WebSocket](https://developer.mozilla.org/pt-BR/docs/Web/API/WebSockets_API)
        - Serialização
            - [Protobuf Buffer](https://developers.google.com/protocol-buffers)
            - [gob](https://go.dev/blog/gob)
            - [msgpack](https://msgpack.org/)
            - [bson](https://www.mongodb.com/docs/manual/reference/bson-types/)
            - [Avro](https://avro.apache.org/)
            - [Thrift](https://thrift.apache.org/)
            - [json](https://www.json.org/json-en.html)
            - [xml](https://pt.wikipedia.org/wiki/XML)
        - [tcp](https://pt.wikipedia.org/wiki/Protocolo_de_controle_de_transmiss%C3%A3o)
        - [udp](https://pt.wikipedia.org/wiki/Protocolo_de_datagrama_do_usu%C3%A1rio)
        - [http](https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Overview)
        - [http2](https://developers.google.com/web/fundamentals/performance/http2?hl=pt-br)
        - [http3](https://pt.wikipedia.org/wiki/HTTP/3)
        - [MQTT](https://mqtt.org/)
