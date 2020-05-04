# Awesome gRPC [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

[<img src="https://cdn.rawgit.com/grpc/grpc.github.io/master/img/grpc.svg" align="right">](https://grpc.io)

> A curated list of useful resources for gRPC


## Contents

- [Documentation](#documentation)
- [Community](#community)
- [Official Libraries and Tools](#official)
- [Tools](#tools)
  * [CLI](#tools-cli)
  * [GUI](#tools-gui)
  * [Testing](#tools-test)
  * [Other](#tools-other)
- [Language-Specific](#lang)
  * [Go](#lang-go)
  * [Node.js](#lang-nodejs)
  * [Java](#lang-java)
  * [Ruby](#lang-ruby)
  * [Python](#lang-py)
  * [C#](#lang-cs)
  * [Rust](#lang-rust)
  * [Haskell](#lang-hs)
  * [Erlang](#lang-erlang)
  * [Elixir](#lang-elixir)
  * [Elm](#lang-elm)
  * [TypeScript](#lang-ts)
  * [Scala](#lang-scala)
  * [Dart](#lang-dart)
  * [Kotlin](#lang-kotlin)
  * [Perl](#lang-perl)
- [Resources](#resources)
  * [Tutorials](#res-tuts)
  * [Videos](#res-videos)
  * [Slides](#res-slides)
  * [Examples](#res-examples)
  * [Miscellaneous](#res-misc)
- [Protocol Buffers](#proto)
  * [Documentation](#proto-docs)
  * [Tools](#proto-tools)
- [Similar](#similar)

## Documentation

- [Website](https://grpc.io/) - Official documentation, libraries, resources, samples and FAQ
- [Technical documentation](https://github.com/grpc/grpc/tree/master/doc) - Collection of useful technical documentation
- [gRPC status codes](https://github.com/grpc/grpc/blob/master/doc/statuscodes.md) - Status codes and their use in gRPC
- [gRPC status code mapping](https://github.com/grpc/grpc/blob/master/doc/http-grpc-status-mapping.md) - HTTP to gRPC Status Code Mapping
- [grpc-errors](https://github.com/avinassh/grpc-errors) - Code examples in each language on how to return and handle error statuses.
- [API Design Guide](https://cloud.google.com/apis/design/) - Google Cloud API Design Guide useful for gRPC API design insights

## Community

- [Community links](https://grpc.io/community/) - Mailing list, Gitter, Twitter, Reddit

<a name="official"></a>
## Official Libraries and Tools

- [gRPC Core](https://github.com/grpc/grpc) - C, C++, Ruby, Node.js, Python, PHP, C#, Objective-C
- [gRPC Java](https://github.com/grpc/grpc-java) - The Java gRPC implementation. HTTP/2 based RPC
- [gRPC Node.js](https://github.com/grpc/grpc-node) - gRPC for Node.js
- [gRPC Go](https://github.com/grpc/grpc-go) - The Go language implementation of gRPC. HTTP/2 based RPC
- [gRPC Swift](https://github.com/grpc/grpc-swift) - The Swift language implementation of gRPC
- [gRPC Dart](https://github.com/grpc/grpc-dart) - The Dart language implementation of gRPC
- [gRPC C#](https://github.com/grpc/grpc-dotnet) - The C# language implementation of gRPC
- [gRPC Web](https://github.com/grpc/grpc-web) - gRPC for Web Clients
- [gRPC Ecosystem](https://github.com/grpc-ecosystem) - gRPC Ecosystem that complements gRPC
- [gRPC contrib](https://github.com/grpc/grpc-contrib) - Known useful contributions around github
- [Homebrew gRPC](https://github.com/grpc/homebrew-grpc) - gRPC formulae repo for Homebrew
- [grpc_cli](https://github.com/grpc/grpc/blob/master/doc/command_line_tool.md) - gRPC CLI tool

## Tools

<a name="tools-cli"></a>
### CLI

- [polyglot](https://github.com/grpc-ecosystem/polyglot) - A gRPC command line client written in Java
- [grpcc](https://github.com/njpatel/grpcc) - Node.js grpc command-line client
- [gcall](https://github.com/bojand/gcall) - Simple Node.js gRPC command line interface
- [Evans](https://github.com/ktr0731/evans) - more expressive universal gRPC (CLI) client
- [grpcurl](https://github.com/fullstorydev/grpcurl) - Like cURL, but for gRPC: Command-line tool for interacting with gRPC servers
- [protodot](https://github.com/seamia/protodot) - Transforming your .proto files into .dot files (and .svg, .png if you happen to have graphviz installed)

<a name="tools-gui"></a>
### GUI

- [letmegrpc](https://github.com/gogo/letmegrpc) - Generate a web form gui from a grpc specification
- [omgRPC](https://github.com/troylelandshields/omgrpc) (Deprecated) - A GUI client for interacting with gRPC services, similar to what Postman is for REST APIs
- [grpcui](https://github.com/fullstorydev/grpcui) - An interactive web UI for gRPC, along the lines of postman (also, a Go library for embedding these web UIs into Go HTTP servers)
- [BloomRPC](https://github.com/uw-labs/bloomrpc) - A nice and simple GUI Client. Exploring and interacting with gRPC services has never been simpler, Inspired By GraphQL-Playground and Postman
- [gRPCox](https://github.com/gusaul/grpcox) - Like Postman, but for gRPC. web based GUI Client for gRPC, extremely easy to use.
- [MuninRPC](https://github.com/muninrpc/muninrpc) - Protobuf request and response testing application under the gRPC system.
- [Delivery](https://github.com/kfwerf/delivery) - A simple electron app for gRPC that uses gRPCurl to autodetect all endpoints/methods and their request bodies, just modify the JSON body. Simplicity in mind.
- [(Yodelay.io)](https://github.com/oslabs-beta/Yodelay) - A browser GUI Making sure your outbound 🗣️ ‘yodelay’ returns the ‘IiiOoo’ 📣 that you expect.

<a name="tools-test"></a>
### Testing

- [ghz](https://github.com/bojand/ghz) - Simple gRPC benchmarking and load testing tool inspired by hey and grpcurl
- [gatling-grpc](https://github.com/phiSgr/gatling-grpc) - A [Gatling](http://gatling.io/) stress test plugin for gRPC.
- [strest-grpc](https://github.com/BuoyantIO/strest-grpc) - A load tester for stress testing grpc intermediaries.
- [hazana](https://github.com/emicklei/hazana) - A Go package for creating load test tooling. Supports gRPC.
- [fortio](https://github.com/fortio/fortio) - A microservices (http, grpc) load testing library and tool from Istio project.
- [grpc-swagger](https://github.com/grpc-swagger/grpc-swagger) - Debugging gRPC application with swagger-ui.
- [grpc-tools](https://github.com/bradleyjkemp/grpc-tools) - A suite of gRPC debugging tools. Like Fiddler/Charles but for gRPC.
- [jmeter-grpc-plugin](https://github.com/zalopay-oss/jmeter-grpc-plugin) - A plugin supports load test gRPC service with Jmeter

<a name="tools-other"></a>
### Other

- [kafka-pixy](https://github.com/mailgun/kafka-pixy) - gRPC/REST proxy for Kafka
- [grpc-proxy](https://github.com/mwitkow/grpc-proxy) - gRPC reverse proxy with the goal of making it easy to expose gRPC services over the internet
- [ratelimit](https://github.com/lyft/ratelimit) - Go/gRPC service designed to enable generic rate limit scenarios from different types of applications
- [ProfaneDB](https://gitlab.com/ProfaneDB/ProfaneDB) - A Protocol Buffers database with gRPC API, built in C++ on top of RocksDB
- [danby](https://github.com/ericbets/danby) - A grpc proxy for the browser
- [docker-protoc](https://github.com/namely/docker-protoc) - Dockerized protoc, grpc-gateway, and grpc_cli commands bundled with Google API libraries
- [grpc-json-proxy](https://github.com/jnewmano/grpc-json-proxy) - A proxy which allows existing tools like Postman or curl to interact with gRPC servers
- [protoc-gen-gotemplate](https://github.com/moul/protoc-gen-gotemplate) - Generic generator based on golang's template system
- [grpc-http-proxy](https://github.com/mercari/grpc-http-proxy) - A reverse proxy server which translate JSON HTTP requests to gRPC calls based on protoreflect
- [grpc-mate](https://github.com/gdong42/grpc-mate) - A dynamic proxy server that translates JSON HTTP requests into gRPC calls
- [jawlb](https://github.com/joa/jawlb) - An unsophisticated grpclb load balancer implementation for Kubernetes and gRPC
- [protoc-gen-hbs](https://github.com/gponsinet/protoc-gen-hbs) - Fast and easy protobuf generation with handlebars and some helpers

<a name="lang"></a>
## Language-Specific

<a name="lang-go"></a>
### Go
- [go-GRPC Micro](https://github.com/micro/go-grpc) - [Micro](https://github.com/micro) based gRPC framework for microservices
- [go-kit gRPC](https://github.com/go-kit/kit/tree/master/transport/grpc) - [Go Kit](https://github.com/go-kit) with gRPC as transport
- [gRPC over NATS](https://github.com/rapidloop/nrpc) - nRPC is an RPC framework like gRPC, but for NATS.
- [grpc-web](https://github.com/improbable-eng/grpc-web) - gRPC Web implementation for Golang and TypeScript
- [grpc-web-devtools](https://github.com/SafetyCulture/grpc-web-devtools) - Chrome Browser extension to aid gRPC-Web development
- [rpcx](https://github.com/smallnest/rpcx) - A RPC service framework based on net/rpc like alibaba Dubbo and weibo Motan
- [grpclb](https://github.com/bsm/grpclb) - External Load Balancing Service solution for gRPC written in Go
- [grpc-proxy](https://github.com/mwitkow/grpc-proxy) - gRPC proxy is a Go reverse proxy that allows for rich routing of gRPC calls with minimum overhead
- [go-microservice-helpers](https://github.com/google/go-microservice-helpers) - A collection of handy snippets that simplify creation of gRPC servers and clients
- [lile](https://github.com/lileio/lile) - Easily create gRPC services in Go
- [proteus](https://github.com/src-d/proteus) - Generate .proto files from Go source code
- [protoc-gen-cobra](https://github.com/fiorix/protoc-gen-cobra) - Command line tool generator for Go gRPC
- [gRPC over WebSocket](https://github.com/glerchundi/grpc-boomerang) - connect to a gRPC Server behind a firewall by using a pre-established WebSocket connection
- [yarpc](https://github.com/yarpc/yarpc-go) - A message passing platform for Go, including support for gRPC
- [promgrpc](https://github.com/piotrkowalczuk/promgrpc) - Prometheus instrumentation for gRPC based services
- [protoreflect](https://github.com/jhump/protoreflect) - Reflection (Rich Descriptors) for Go Protocol Buffers
- [grpchan](https://github.com/fullstorydev/grpchan) - Channels for gRPC: custom transports, such as in-process and HTTP 1.1
- [grpcui](https://github.com/fullstorydev/grpcui) - Embed a gRPC web UI into a Go gRPC/HTTP server
- [clay](https://github.com/utrack/clay) - Minimal server platform for gRPС+REST+Swagger APIs
- [grpc-consul-resolver](https://github.com/mbobakov/grpc-consul-resolver) - Easy to use endpoints resolver for the services registered in the [Consul](https://www.consul.io/)
- [kuberesolver](https://github.com/sercand/kuberesolver) - gRPC Load Balancer with Kubernetes resolver
- [ttrpc](https://github.com/containerd/ttrpc) - GRPC for low-memory environments
- [grapi](https://github.com/izumin5210/grapi) - 😮 A surprisingly easy API server and generator in gRPC and Go
- [gripmock](https://github.com/tokopedia/gripmock) - gRPC Mock Server
- [grpc-gateway-boilerplate](https://github.com/johanbrandhorst/grpc-gateway-boilerplate) - All the boilerplate you need to get started with writing grpc-gateway powered REST services in Go
- [protoc-gen-struct-transformer](https://github.com/bold-commerce/protoc-gen-struct-transformer) - Transformation function generator for protocol buffers.
- [cmux](https://github.com/soheilhy/cmux) - Connection multiplexer for GoLang: serve different services on the same port! Supports gRPC.
- [go-grpc-channelz](https://github.com/rantav/go-grpc-channelz) - A channelz UI for Golang. Channelz is an approved and already implemented proposal describing the inner state of gRPC connections/channels. go-grpc-channelz provides a simple UI for channelz for easy diagnosis.
- [goprotoc](https://github.com/jhump/goprotoc) - Library for writing protoc plugins in Go; also includes a pure-Go protoc replacement.
- [gRPC for production](https://github.com/apssouza22/grpc-server-go) - A Golang project that provides the core requirements for a production-ready gRPC communication.
- [protoc-gen-mock](https://github.com/carvalhorr/protoc-gen-mock) - A protoc plugin to generate gRPC mock services from proto definitions in Golang

<a name="lang-nodejs"></a>
### Node.js
- [Mali](https://github.com/malijs/mali) - A minimalistic gRPC microservice framework for Node.js
- [grpc-host-builder](https://github.com/litichevskiydv/grpc-host-builder) - Lightweight library for building gRPC services with server side interceptors support
- [grpc-caller](https://github.com/bojand/grpc-caller) - An improved Node.js gRPC client
- [grpc-create-metadata](https://github.com/bojand/grpc-create-metadata) - Helper utility for creating gRPC `Metadata`
- [grpc-create-error](https://github.com/bojand/grpc-create-error) - Utility function for creating `Errors` for gRPC responses
- [grpc-error](https://github.com/bojand/grpc-error) - `GRPCError` class that wraps `create-grpc-error`
- [grpc-inspect](https://github.com/bojand/grpc-inspect) - gRPC protocol buffer inspection utility
- [Node.js Proto Files](https://github.com/googleapis/nodejs-proto-files) - All of the Google API's protocol buffer files
- [grpc-bus](https://github.com/paralin/grpc-bus) - Call gRPC services (even streams!) from the browser over any two-way socket to Node and soon Go
- [grpc-errors](https://github.com/ortoo/grpc-errors) - A quick and easy way of generating errors for use with grpc
- [grpc-dynamic-gateway](https://github.com/konsumer/grpc-dynamic-gateway) - Like grpc-gateway, but written in node and dynamic.
- [node-protoc-plugin](https://github.com/konsumer/node-protoc-plugin) - Create protoc code-generation plugins easily in nodejs.
- [grpc-promise](https://github.com/carlessistare/grpc-promise) - GRPC promisify module for all Request/Response types: standard and stream
- [firecomm](https://github.com/firecomm/firecomm) - Feature library for gRPC-Node
- [grpc-web-gateway](https://github.com/dialogs/grpc-web-gateway) – HTTP & WebSocket proxy gateway for gRPC services

<a name="lang-java"></a>
### Java

- [gax-java](https://github.com/googleapis/gax-java) - Google API Extensions for Java
- [Armeria](https://github.com/line/armeria) - Asynchronous RPC/REST library built on top of Java 8, Netty, HTTP/2, Thrift and gRPC
- [grpc-spring-boot-starter](https://github.com/yidongnan/grpc-spring-boot-starter) - Spring Boot starter module for gRPC framework
- [grpc-spring-boot-starter](https://github.com/LogNet/grpc-spring-boot-starter) Spring Boot starter module for gRPC framework from LogNet.
- [reactive-grpc](https://github.com/salesforce/reactive-grpc) - Integrates reactive programming with grpc-java
- [grpc-java-contrib](https://github.com/salesforce/grpc-java-contrib) - Useful extensions for the grpc-java library
- [rejoiner](https://github.com/google/rejoiner) - Generates a GraphQL schema from gRPC microservices
- [hoverfly-java-grpc](https://mvnrepository.com/artifact/io.specto/hoverfly-java-grpc) - MITM proxy for recording and simulating gRPC services

<a name="lang-ruby"></a>
### Ruby

- [gruf](https://github.com/bigcommerce/gruf) - gRPC Ruby Framework
- [gapic-generator-ruby](https://github.com/googleapis/gapic-generator-ruby) - Generates Ruby gRPC client libraries from protocol buffer definitions of an API.

<a name="lang-py"></a>
### Python

- [grpclib](https://github.com/vmagamedov/grpclib) - Pure-Python gRPC implementation, based on hyper-h2 project
- [pytest-grpc](https://github.com/kataev/pytest-grpc) - pytest plugin which allow test gRPC services
- [grpcalchemy](https://github.com/GuangTianLi/grpcalchemy) - The Python micro framework for building gPRC application
- [django-grpc](https://github.com/gluk-w/django-grpc) - Django application to build gRPC services with access to ORM, settings and everything else
- [garuda](https://github.com/dhilipsiva/garuda) - Automagically Exposing Djagno ORM over gRPC for microservices written in any other languages

<a name="lang-cs"></a>
### C#

- [MagicOnion](https://github.com/neuecc/MagicOnion) - gRPC based HTTP/2 RPC Streaming Framework for .NET, .NET Core and Unity
- [Grpc.Tools](https://www.nuget.org/packages/Grpc.Tools/) - gRPC and Protocol Buffer compiler for managed C# and native C++ projects. See [Introduction to gRPC on .NET Core](https://docs.microsoft.com/en-us/aspnet/core/grpc/?view=aspnetcore-3.0) tutorial.

<a name="lang-rust"></a>
### Rust

- [grpc-rs](https://github.com/pingcap/grpc-rs) - The gRPC library for Rust built on C Core library and futures
- [grpc-rust](https://github.com/stepancheg/grpc-rust) - Rust implementation of gRPC
- [tower-grpc](https://github.com/tower-rs/tower-grpc) - A client and server gRPC implementation based on Tower
- [tonic](https://github.com/hyperium/tonic) - A native gRPC client & server implementation with async/await support

<a name="lang-hs"></a>
### Haskell

- [grpc-haskell](https://github.com/grpc/grpc-haskell) - gRPC library binding for Haskell

<a name="lang-erlang"></a>
### Erlang

- [Erlang grpc](https://github.com/bluehouse-technology/grpc) - Erlang library for gRPC
- [grpcbox](https://github.com/tsloughter/grpcbox) - Erlang grpc client and server
- [bert](https://github.com/synrc/bert) - Erlang Google Protobuf V3 generator from HRL files

<a name="lang-elixir"></a>
### Elixir

- [grpc-elixir](https://github.com/tony612/grpc-elixir) - The Elixir implementation of gRPC

<a name="lang-elm"></a>
### Elm

- [elm-protobuf](https://github.com/tiziano88/elm-protobuf) - Protoc plugin generating elm code from proto definitions

<a name="lang-ts"></a>
### TypeScript

- [ts-protoc-gen](https://github.com/improbable-eng/ts-protoc-gen) - Protoc Plugin for TypeScript Declarations
- [protoc-gen-tstypes](https://godoc.org/github.com/tmc/grpcutil/protoc-gen-tstypes) - Configurable Protoc Plugin to generate TypeScript types.

<a name="lang-scala"></a>
### Scala

- [ScalaPB](https://scalapb.github.io/) - Protocol Buffer Compiler for Scala
- [Akka-gRPC](https://developer.lightbend.com/docs/akka-grpc/current/) - Akka gRPC provides support for building streaming gRPC servers and clients on top of Akka Streams.
- [Mu](https://higherkindness.io/mu/) - Mu RPC is a purely functional library for building RPC endpoint-based services with support for gRPC and HTTP/2

<a name="lang-dart"></a>
### Dart

- [grpc-dart](https://pub.dartlang.org/packages/grpc) - Protocol Buffer Compiler for Dart

<a name="lang-kotlin"></a>
### Kotlin

- [kroto-plus](https://github.com/marcoferrer/kroto-plus) - gRPC Coroutines Integration and Protobuf message DSL support
- [grpc-kotlin](https://github.com/rouzwawi/grpc-kotlin) - A protoc plugin for generating native Kotlin bindings using coroutine primitives for gRPC services
- [gapic-generator-kotlin](https://github.com/googleapis/gapic-generator-kotlin) - Generates coroutine-based gRPC Kotlin client libraries from a protocol buffer description of an API
- [grpc-kapt](https://github.com/google/grpc-kapt) - Annotation driven gRPC clients & servers in Kotlin with coroutines

<a name="lang-perl"></a>
### Perl

- [grpc-perl](https://github.com/joyrex2001/grpc-perl) - Experimental Perl gRPC library supporting grpc client

## Resources

<a name="res-tuts"></a>
### Tutorials

- [Building a gRPC service with Node.js](https://codelabs.developers.google.com/codelabs/cloud-grpc/index.html) - Google Cloud Platform Codelab
- [Getting Started with Microservices using Go, gRPC and Kubernetes](https://outcrawl.com/getting-started-microservices-go-grpc-kubernetes/)
- [gRPC in Production](https://about.sourcegraph.com/go/grpc-in-production-alan-shreve/)
- [gRPC Go: Beyond the basics](https://blog.gopheracademy.com/advent-2017/go-grpc-beyond-basics/) - GopherAcademy article
- [Building High Performance APIs In Go Using gRPC](http://www.agiratech.com/building-high-performance-apis-go-grpc/) - Small tutorial on building a simple API using gRPC and Go
- [Bidirectional gRPC streaming for Go](https://rakyll.org/grpc-streaming/)
- [How We Build gRPC Services At Namely](https://medium.com/namely-labs/how-we-build-grpc-services-at-namely-52a3ae9e7c35) - Blog article from Namely Labs
- [Our experience designing and building gRPC services](https://blog.bugsnag.com/using-grpc-in-production/) - Blog series from Bugsnag on building a new Releases dashboard backend using gRPC
- [Writing gRPC Interceptors in Go](https://medium.com/@shijuvar/writing-grpc-interceptors-in-go-bf3e7671fe48) - A simple tutorial on gRPC Interceptors
- [An introduction to gRPC](https://devopedia.org/grpc)
- [How we use gRPC to build a client/server system in Go](https://medium.com/pantomath/how-we-use-grpc-to-build-a-client-server-system-in-go-dd20045fa1c2) - A technical presentation on how to use gRPC (and Protobuf) to build a robust client/server system
- [Serving gRPC and HTTP services on the same port](https://www.d3void.net/post/grpc-with-http/) - Small tutorial on how to serve http and gRPC on same port in Go
- [Take a REST with HTTP/2, Protobufs, and Swagger](https://coreos.com/blog/grpc-protobufs-swagger.html) - Small tutorial on how to serve http and gRPC on same port in Go
- [OpenCensus for Go gRPC developers](https://medium.com/@orijtech/opencensus-for-go-grpc-developers-7f3ee1ac3d6d) - Tutorial on how to use OpenCensus with gRPC and Go. Also available for [Java](https://medium.com/@orijtech/opencensus-for-java-grpc-developers-23c25de0a057) and [Python](https://medium.com/@orijtech/opencensus-for-python-grpc-developers-9e460e054395).
- [How to develop Go gRPC microservice with HTTP/REST endpoint, middleware, Kubernetes deployment, etc](https://medium.com/@amsokol.com/tutorial-how-to-develop-go-grpc-microservice-with-http-rest-endpoint-middleware-kubernetes-daebb36a97e9) - A series of blog posts for gRPC development using Go. [Source code](https://github.com/amsokol/go-grpc-http-rest-microservice-tutorial).
- [GopherJS Client and gRPC Server](https://jbrandhorst.com/post/gopherjs-client-grpc-server/) - A guide to implementing a GopherJS frontend to a gRPC backend exposed over HTTP via the gRPC-gateway. Also available [related gRPC-Web with GopherJS tutorial](https://jbrandhorst.com/post/gopherjs-grpcweb/).
- [The G-Unit Stack: Go, GraphQL, and gRPC](https://iheanyi.com/journal/2018/05/12/the-g-unit-stack-go-graphql-and-grpc/) - A blog post and tutorial on using Go, GraphQL and gRPC. Associated [repo](https://github.com/iheanyi/go-grpc-graphql-simple-example).
- [Envoy, gRPC, and Rate Limiting](https://venilnoronha.io/envoy-grpc-and-rate-limiting) - A tutorial on using gRPC and Envoy to build a rate limit service - [Venil Noronha](https://venilnoronha.io), VMware Open Source Technology Center
- [Seamless Cloud-Native Apps with gRPC-Web and Istio](https://venilnoronha.io/seamless-cloud-native-apps-with-grpc-web-and-istio) - A tutorial on building a Cloud-Native web app using gRPC-Web and Istio - [Venil Noronha](https://venilnoronha.io), VMware Open Source Technology Center
- [Backward and Forward Compatibility, Protobuf Versioning, Serialization](https://www.beautifulcode.co/backward-and-forward-compatibility-protobuf-versioning-serialization) - A small article on making gRPC API changes
- [Node, gRPC, and Postgres](https://mherman.org/blog/node-grpc-postgres/) - This tutorial looks at how to implement an API with Node, gRPC, and Postgres.
- [Building High Performance APIs In Go Using gRPC And Protocol Buffers](https://medium.com/@shijuvar/building-high-performance-apis-in-go-using-grpc-and-protocol-buffers-2eda5b80771b) - An introductory gRPC Go tutorial.
- [Understanding gRPC](https://www.vineethweb.com/post/grpc/) - An introductory gRPC tutorial with example application in Go.
- [Part 1: Demystifying gRPC](https://dev-state.com/posts/grpc_framework_1/) - A simple gRPC service with context cancelation and secure connection over SSL/TLS.
- [Part 2: Demystifying gRPC](https://dev-state.com/posts/grpc_framework_2/) - Extend the service with gRPC streaming and Python backend.
- [Part 3: Demystifying gRPC](https://dev-state.com/posts/grpc_framework_3/) - Add Unary and Stream gRPC Interceptors to a service and provide REST endpoints with grpc-gateway.
- [gRPC in Microservices](https://milad.dev/posts/grpc-in-microservices/) - Tutorial on using gRPC in microservice architetures.

<a name="res-videos"></a>
### Videos

- [gRPC: Google's high-performance, open-source RPC framework](https://www.youtube.com/watch?v=sZx3oZt7LVg) - GothamGo 2015 by Sameer Ajmani
- [Introduction to gRPC: A general RPC framework that puts mobile and HTTP/2 first](https://www.youtube.com/watch?v=kUz2zjkKxFg) - Devoxx by Mete Atamel
- [gRPC: The Story of Microservices at Square](https://www.youtube.com/watch?v=-2sWDr3Z0Wo) - Apigee webcast
- [Scalable Realtime Microservices with Kubernetes and gRPC](https://www.youtube.com/watch?v=xb8u2s7cxzg) - Mark Mandel @ Google
- [Text to Speech server with gRPC and Kubernetes](https://www.youtube.com/watch?v=XaMr--wAuSI) - justforfunc #12
- [GRPC Microservices 101](https://www.youtube.com/watch?v=-t57ZQZpjqs) - Google Developer Group Washington by Ray Tsang
- [Efficient Microservices w/ Binary Protocol - gRPC 101](https://www.youtube.com/watch?v=RqK-mwh3-aY) - By Ray Tsang
- [grpc: From Tutorial to Production](https://www.youtube.com/watch?v=7FZ6ZyzGex0) - GopherCon 2017 by Alan Shreve
- [Scalable Microservices with gRPC, Kubernetes, and Docker](https://www.youtube.com/watch?v=xsIwYL-N4vI) - Node Interactive 2016 by Sandeep Dinesh
- [Building Microservices w/gRPC & Kubernetes](https://www.youtube.com/watch?v=27swR9HACWU) - Philly ETE 2016 #49 by Kelsey Hightower
- [Building high performance microservices with Kubernetes, Go, and gRPC](https://www.youtube.com/watch?v=YiNt4kUnnIM) - Google Cloud Next '17 by Andrew Jessup
- [Modifying gRPC Services Over Time](https://www.youtube.com/watch?v=F2WYEFLTKEw) - Eric Anderson, Google at KubeCon + CloudNativeCon 2017 - Austin
- [Next Generation Services at Indeed Using gRPC](https://www.youtube.com/watch?v=aQ2d9iLDR8Y) - Jaye Pitzeruse, Indeed.com at KubeCon + CloudNativeCon 2017 - Austin
- [Generating Unified APIs with Protocol Buffers and gRPC](https://www.infoq.com/presentations/api-pb-grpc) - A video on Protocol Buffers, gRPC and Envoy from Lyft.
- [Intro to gRPC: A Modern Toolkit for Microservice Communication](https://www.youtube.com/watch?v=RoXT_Rkg8LA) - A video from Twilio's Signal Conference
- [gRPC and Go: Developing Efficient and Type-Safe Services](https://www.youtube.com/watch?v=J-NTfvYL_OE)
- [Best Practices for (Go) gRPC Services](https://www.youtube.com/watch?v=Z_yD7YPL2oE)
- [Creating GopherJS Apps with gRPC-Web](https://www.youtube.com/watch?v=R2HaxH7Et64) - At FOSDEM
- [justforfunc #31: gRPC Basics](https://www.youtube.com/watch?v=uolTUtioIrc) - JustForFunc: Programming in Go series Episode 31 covering gRPC
- [Efficient service communication with gRPC](https://www.youtube.com/watch?v=t9SUcf3Uwlg) - Talk at microXchg 2018 Berlin
- [gRPC Java Course on Udemy](http://bit.ly/grpc-java-github) - Online Course (4 hours) that walks through several examples and implementations of gRPC using the Java Language
- [HTTP and JSON for your gRPC Services - Michael Hamrah](https://www.youtube.com/watch?v=AmXo6tPGUdQ) - from Full Stack Fest
- [Types All the Way Down — gRPC and Go Infrastructure at Lyft](https://www.youtube.com/watch?v=ZqPTKJu2QFk) - Christopher Burnett  at Istanbul Tech Talks
- [Using gRPC for Long-lived and Streaming RPCs](https://www.youtube.com/watch?v=Naonb2XD_2Q) - Eric Anderson, Google at KubeCon North America 2018
- [Intro: gRPC-Web](https://www.youtube.com/watch?v=RtyKEDZipsM) - Stanley Cheung & Wenbo Zhu, Google at at KubeCon North America 2018
- [gRPC Loadbalancing on Kubernetes](https://www.youtube.com/watch?v=F2znfxn_5Hg) - Presentation at KubeCon Europe 2018. [Source](https://github.com/jtattermusch/grpc-loadbalancing-kubernetes-examples).
- [Putting gRPC in Practice](https://www.youtube.com/watch?v=8KWmNw9jQ04) - Presentation on working with gRPC.
- [The Story of Why We Migrate to gRPC and How We Go About It](https://www.youtube.com/watch?v=fMq3IpPE3TU) - Matthias Grüter, Spotify at KubeCon + CloudNativeCon Europe 2019
- [Authentication and Security in gRPC Microservices](https://www.youtube.com/watch?v=_y-lzjdVEf0) - Jan Tattermusch, Google at KubeCon + CloudNativeCon Europe 2019
- [JustFootball’s Journey to gRPC + Linkerd in Production](https://www.youtube.com/watch?v=AxPfa7Mp_WY) - Ben Lambert, & Kevin Lingerfelt at KubeCon + CloudNativeCon Europe 2019
- [gRPC load balancing and Service Mesh](https://www.youtube.com/watch?v=FuXnfGHUZcU) - Vishal Powar, Google at KubeCon + CloudNativeCon Europe 2019
- [Adopting gRPC: Overcoming Team and Technical Hurdles](https://www.youtube.com/watch?v=VNllljvhcnk) - GOTO 2019 • Adopting gRPC: Overcoming Team and Technical Hurdles • Josh Humphries
- [Moving to gRPC Java](https://www.youtube.com/watch?v=vFBuvWVIcYQ) - Mya Pitzeruse at Indeed.com

<a name="res-slides"></a>
### Slides

- [gRPC Overview](http://www.slideshare.net/VarunTalwar4/grpc-overview) - An overview at gRPC: Talk at Slack by
Varun Talwar
- [gRPC Design and Implementation](https://www.slideshare.net/VarunTalwar4/grpc-design-and-implementation) - April 2016 talk at Stanford by Varun Talwar
- [gRPC - boilerplate to high-performance scalable APIs](https://www.slideshare.net/AboutYouGmbH/robert-kubis-grpc-boilerplate-to-highperformance-scalable-apis-codetalks-2015) - code.talks 2015 by Robert Kubis
- [HTTP2 and gRPC](https://www.slideshare.net/GuoJing8/http2-and-grpc) - A simple introduction about HTTP2 and gRPC by Xin Gong Chang
- [gRPC and Microservices](https://www.slideshare.net/blinkingsquirrel/grpc-and-microservices) - Overview of Google's open source microservices framework - gRPC, based on HTTP2 and protocol buffers. Presented at Golang Melbourne, June 2016 by Jonathan Gomez
- [gRPC and Microservices](https://github.com/jonog/talks/blob/master/src/grpc/grpc-presentation.md) - Golang Melbourne - June 2016 Go Hack Night by Jonathan Gomez
- [Scalable Microservices with gRPC, Kubernetes, and Containers](https://speakerdeck.com/googlecloudplatform/scalable-microservices-with-grpc-kubernetes-and-containers-devfest-ukraine) - DevFest Ukraine
- [OpenAPI and gRPC Side by-Side](https://www.slideshare.net/timburks/openapi-and-grpc-side-byside) - APIStrat Conference -
Tim Burks
- [Go+Microservices at Mercari](https://talks.godoc.org/github.com/tcnksm/talks/2017/11/gocon2017/gocon2017.slide) - Taichi Nakashima at Go Conference 2017
- [gRPC - RPC rebirth?](https://www.slideshare.net/LusBarbosa9/grpcrpc-rebirth) - Presentation about gRPC at the 23. NetPonto community meeting in Porto by Luís Barbosa

<a name="res-examples"></a>
### Examples

- [gifinator](https://github.com/GoogleCloudPlatform/gifinator) - A sample application demonstrating Kubernetes, gRPC, Go and cute Gophers demoed at Google GCP Next 2017
- [Text to Speech server with gRPC and Kubernetes](https://github.com/campoy/justforfunc/tree/master/12-say-grpc) - justforfunc #12
- [Multiplayer Simon Says - A Game using gRPC and Kubernetes](https://github.com/grpc-ecosystem/grpc-simon-says) - Sample app with Go server and clients using Node.js (on Arduino and web), and Java (Android and CLI)
- [Go Microservices Example](https://github.com/harlow/go-micro-services) - HTTP up front, Protobufs in the rear
- [Streaming RPC's using gRPC](https://github.com/ridha/grpc-streaming-demo) - A quick demo of bi-directional streaming RPC's using grpc, Go and Python
- [gRPC Java Examples](https://github.com/saturnism/grpc-java-by-example) - A collection of useful/essential gRPC Java Examples
- [gRPC/OpenCensus Demo](https://github.com/rakyll/opencensus-grpc-demo) - Export metrics and traces from gRPC servers and clients using Java, Go and Prometheus
- [go-micro-services](https://github.com/harlow/go-micro-services) - An demonstration of Golang micro-services that expose a HTTP/JSON frontend and then leverages gRPC for inter-service communication
- [Colossus](https://github.com/lucperkins/colossus) - An example multi-language gRPC microservice architecture built by Bazel and targeting Kubernetes
- [coolstore-microservices](https://github.com/vietnam-devs/coolstore-microservices) - A containerized polyglot gRPC microservices based on .NET Core, Nodejs and more running on Istio
- [gRPC Microservices with Go and Kubernetes](https://github.com/shuza/kubernetes-go-grpc) - A sample application use gRPC in microservice and deploy in kubernetes.

<a name="res-misc"></a>
### Miscellaneous

- [gRPC with Load Balancer or Proxy or on AWS](https://gist.github.com/bojand/6a604f7e369d7c7d8c39eb77878a42c2) - Various notes on doing gRPC behind a load balancer or proxy or on AWS
- [gRPC service upgrade, versioning](https://groups.google.com/forum/#!topic/grpc-io/LPsPg5ctQd4) - A short possibly useful discussion on gRPC service upgrade and versioning
- [Packaging Generated Code for gRPC Services](https://blog.bugsnag.com/libraries-for-grpc-services/) - An article demonstrating a strategy on how to version and package gRPC libraries
- [Migrating APIs from REST to gRPC at WePay](https://wecode.wepay.com/posts/migrating-apis-from-rest-to-grpc-at-wepay) - A blog post on migrating from REST to gRPC

<a name="proto"></a>
## Protocol Buffers

<a name="proto-docs"></a>
### Documentation

- [Website](https://developers.google.com/protocol-buffers/) - Official website and documentation
- [Third-Party Add-ons for Protocol Buffers](https://github.com/protocolbuffers/protobuf/blob/master/docs/third_party.md) - List of add-ons for Protocol Buffers in main github repository

<a name="proto-tools"></a>
### Tools

- [buf](https://buf.build) - Protobuf tool that includes linting and breaking change detection.
  Allows many types of input including directly checking remote repositories and tarballs, and has a built-in compiler as well.
- [prototools](https://github.com/sourcegraph/prototools) - Documentation generator & other tools for protobuf/gRPC
- [protoc-gen-doc](https://github.com/pseudomuto/protoc-gen-doc) - Documentation generator plugin for Google Protocol Buffers
- [Protoxygen](https://github.com/lisroach/Protoxygen) - [Doxygen](http://doxygen.nl) plugin to generate documentation for protobuf/gRPC
- [openapi2proto](https://github.com/NYTimes/openapi2proto) - A tool for generating Protobuf v3 schemas and gRPC service definitions from OpenAPI specifications
- [Wireshark Protobuf Dissector](https://github.com/128technology/protobuf_dissector) - A Wireshark Lua plugin for decoding Google protobuf packets. [Relevant PR and discussion](https://github.com/google/protobuf/issues/3303).
- [protoc-gen-lint](https://github.com/ckaznocha/protoc-gen-lint) - A plug-in for Google's Protocol Buffers (protobufs) compiler to lint .proto files for style violations
- [prototool](https://github.com/uber/prototool) - Compile, lint, and format Protobuf files, and generate stubs for any lanuguage/plugin, along with Vim/IDE integration
- [protoc-gen-validate](https://github.com/lyft/protoc-gen-validate) - Protoc plugin to generate polyglot message validators
- [go-proto-validators](https://github.com/mwitkow/go-proto-validators) - Generate message validators from .proto annotations, used in `grpc_validator` Go gRPC middleware.
- [protolock](https://github.com/nilslice/protolock) - Protocol Buffer companion tool to `protoc` and `git`. Track your .proto files and prevent changes to messages and services which impact API compatibilty.
- [protoc-gen-map](https://github.com/jackskj/protoc-gen-map) - SQL data mapper framework for Protocol Buffers.
- [api-linter](https://github.com/googleapis/api-linter) - A linter for APIs defined in protocol buffers.
- [protoc-gen-struct-transformer](https://github.com/bold-commerce/protoc-gen-struct-transformer) - Transformation functions generator for Protocol Buffers.

### Similar

- [gogoprotobuf](https://github.com/gogo/protobuf) - Fork of golang/protobuf with extra code generation features
- [MessagePack](http://msgpack.org/index.html) - It's like JSON, but fast and small
- [Thrift](https://thrift.apache.org/) - Thrift is an interface definition language and binary communication protocol
- [TChannel](https://github.com/uber/tchannel) - Network multiplexing and framing protocol for RPC
- [Cap’n Proto](https://capnproto.org/) - Think Protocol Buffers, except faster
- [FlatBuffers](https://google.github.io/flatbuffers/) - An efficient cross platform serialization library
- [RSocket](http://rsocket.io/) - Application protocol providing Reactive Streams semantics
- [Twirp](https://github.com/twitchtv/twirp) - A simple RPC framework with protobuf service definitions
- [Greenpack](https://github.com/glycerine/greenpack) - Serialization format similar to MessagePack, but adds field versioning and type annotation

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

## License

[![CC BY 4.0](https://licensebuttons.net/l/by/4.0/88x31.png)](https://creativecommons.org/licenses/by/4.0/)

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).
