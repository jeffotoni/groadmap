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
    - generics / [T any](s []T)   
    - [constantes](https://gomanual.jeffotoni.com/pages/language_introduction/introduction/constants.html)
    - [variáveis](https://gomanual.jeffotoni.com/pages/language_introduction/introduction/variables.html)
    - [iota](https://gomanual.jeffotoni.com/pages/language_introduction/introduction/iota.html)
    - func init
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
    - [error](https://www.educative.io/edpresso/what-is-type-error-in-golang)
    - [panic](https://gobyexample.com/panic)
    - [recover](https://gobyexample.com/recover)

2. Goroutines
    - [channel](https://gomanual.jeffotoni.com/pages/goroutines/channels.html)
    - [channel buffer](https://gomanual.jeffotoni.com/pages/goroutines/channel_buffering.html)
    - [select](https://gomanual.jeffotoni.com/pages/goroutines/select.html)
    - [sync.Mutex](https://pkg.go.dev/sync#Mutex)
    - [sync.Map](https://pkg.go.dev/sync#Map)
    - [sync.WaitGroup](https://pkg.go.dev/sync#WaitGroup)
    - [sync.Pool](https://pkg.go.dev/sync#Pool)

3. Runtime
    - [runtime.GOMAXPROCS](https://pkg.go.dev/runtime#GOMAXPROCS)
    - [runtime.NumCPU()](https://pkg.go.dev/runtime#NumCPU)   
    - [runtime.NumGoroutine()](https://pkg.go.dev/runtime#NumGoroutine)
    
4. go
    - [go test](https://gomanual.jeffotoni.com/pages/commands/go_test.html)
        - go test -v
        - go test -run ^NameFunc$
        - go test -coverprofile
        - go test ../../
        - go test -bench . -benchmem
        - go test -fuzz=Fuzz

    - go build & go run .
        - [go run .](https://gomanual.jeffotoni.com/pages/commands/go_run.html)
        - go run -race .
        - CGO_ENABLED=0 go build
        - [go build -ldflags="-s -w"](https://gomanual.jeffotoni.com/pages/commands/go_build.html)
        - go build -gcflags '-m -l'
        - GOOS=linux GOARCH=amd64 go build
        - go build GOARCH=wasm GOOS=js go build
        - go build -gcflags -S
        - go help buildmode
        - go build -buildmode=plugin

    - [go install golang.org/x/website/tour@latest](https://gomanual.jeffotoni.com/pages/commands/go_install.html)

5. Modulos
    - package & import
        - import ..
        - import "fml"
        - import "my-pkg/util"
        - package mypkg

    - go.mod
    - go.sum
    - [go mod init](https://gomanual.jeffotoni.com/pages/commands/go_mod.html)
    - go mod tidy
    - go mod vendor
    - go mod download
    - [go env](https://gomanual.jeffotoni.com/pages/commands/go_env.html)
    - GO111MODULE=on
    - GOARCH=amd64
    - GOPRIVATE
    - GOPROXY
    - GOSUMDB

6. Patterns
    - Build
    - Factory Method
    - Abstract Factory
    - Adapter
    - Bridge
    - Facade
    - Composite
    - Decorator
    - Prototype
    - Singleton
    - Template Method

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
            - CORS
            - rate limit
            - logging
            - metrics
            - auth
            - tracing
            - limiter
            - [jwt](https://github.com/golang-jwt/jwt)
            - logger
            - cache
            - Instrumentação
                - [Prometheus](https://github.com/prometheus/prometheus)
                - [Datadog](https://github.com/DataDog/datadog-agent)
                - [New Relic](https://github.com/newrelic/go-agent)
                - [loggly](https://github.com/segmentio/go-loggly)

9. Conhecimentos Prévios
    - [git](https://git-scm.com/)
        - git init
        - git add .
        - git commit 
        - git push
        - git merge
        - git rebase
        - git log
        - git diff
        - git show
        - git clone

    - [docker](https://www.docker.com/)
        - docker run
        - docker build
        - docker images
        - docker push
        - docker login
        - docker ps -a

    - [docker-compose](https://docs.docker.com/compose/)
    - [sql basic syntax](https://www.w3schools.com/sql/sql_syntax.asp)
    - [openssl](https://www.openssl.org/)
    - ssh-keygen
    - https/http
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
