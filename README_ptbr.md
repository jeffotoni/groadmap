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
    - gonstantes, variáveis, iota
    - func init, types
    - funcs, variadic, return multiplos valores
    - closures / funções anônimas
    - array, slice
    - for, switch, if, else, range
    - make, new
    - maps
    - ponteiros, structs, métodos
    - type interface, interface{}
    - defer, error, panic, recover

2. Goroutines
    - channel, channel buffer
    - select
    - sync.Mutex
    - sync.Map
    - sync.WaitGroup
    - sync.Pool

3. Runtime
    - runtime.GOMAXPROCS
    - runtime.NumCPU()   
    - runtime.NumGoroutine()
    
4. go
    - go test
        - go test -v
        - go test -run ^NameFunc$
        - go test -coverprofile
        - go test ../../
        - go test -bench . -benchmem
        - go test -fuzz=Fuzz

    - go build & go run .
        - go run .
        - go run -race .
        - CGO_ENABLED=0 go build
        - go build -ldflags="-s -w"
        - go build -gcflags '-m -l'
        - GOOS=linux GOARCH=amd64 go build
        - go build GOARCH=wasm GOOS=js go build
        - go build -gcflags -S
        - go help buildmode
        - go build -buildmode=plugin

    - go install golang.org/x/website/tour@latest

5. Modulos
    - package & import
        - import ..
        - import "fml"
        - import "my-pkg/util"
        - package mypkg

    - go.mod, go.sum
    - go mod init, go mod tidy
    - go mod vendor, go mod download
    - go env, GO111MODULE=on, GOARCH=amd64
    - GOPRIVATE, GOPROXY, GOSUMDB

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
    81. Server
        - http.NewServeMux, http.Server
        - http.HandlerFunc, http.HandleFunc
        - http.Handle, http.Handler
        - http.Status, next.ServeHTTP
        - ListenAndServe, ListenAndServeTLS
        - http.FileServer, http.Dir, http.StripPrefix
        - Embed, http.FS
        - html/template
            - template.ParseFiles
            - template.Parse
            - template.ParseFS
            - template.New
            - template.Must
            - template.Execute
            - template.ExecuteTemplate

    82. Client
        - http.Transport, http.Client
        - http.Get, http.Post, http.PostForm
        - ioutil.ReadAll(r io.Reader)
        - http.NewRequest, http.NewRequestContext
        - Context.WithCancel

    83. Frameworks Web
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

    84. Routers
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

    85. Middlewares
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
            - jwt
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
