 [![Coverage Status](https://coveralls.io/repos/github/microservices-demo/orders/badge.svg?branch=master)](https://coveralls.io/github/microservices-demo/orders?branch=master)
[![](https://images.microbadger.com/badges/image/weaveworksdemos/orders.svg)](http://microbadger.com/images/weaveworksdemos/orders "Get your own image badge on microbadger.com")[![CodeQL](https://github.com/toomone/orders/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/toomone/orders/actions/workflows/codeql-analysis.yml)

# orders
A microservices-demo service that provides ordering capabilities. It is sub part of the sockshop ecommerce webservices.

This build is built, tested and released by GitHub Action and deploy to Azure Kubernetes Service (AKS).

# API Spec

Checkout the API Spec [here](http://microservices-demo.github.io/api/index?url=https://raw.githubusercontent.com/microservices-demo/orders/master/api-spec/orders.json)

# Build

## Jar
`mvn -DskipTests package`

## Docker
`GROUP=weaveworksdemos COMMIT=test ./scripts/build.sh`

