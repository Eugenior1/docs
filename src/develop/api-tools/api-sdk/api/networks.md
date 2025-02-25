---
sidebar_position: 0
---

# Networks

> Referenced repository: [https://docs.everos.dev/ever-sdk/reference/ever-os-api/networks#networks](https://docs.everos.dev/ever-sdk/reference/ever-os-api/networks#networks)

Each Everscale Operating System (EVER OS) instance has a single GraphQL API endpoint. Each Cloud has several EVER OS instances running for reliability.

## Networks

> **Attention!**
>
> **You need to specify ALL the endpoints in your configuration, not just one from the list. We do not guarantee availability of each endpoint all the time, but we guarantee that at least 1 endpoint is operational at the moment.**

| EVER OS                                                            | Discription                             | Web Playground URLs                                                                                                                                                                                       | HTTP Endpoints                                                                                                                                                         | Websocket Endpoints                                                                                                                                                                                     |
|--------------------------------------------------------------------|-----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| EVER OS Cloud for Everscale                                        | Access to Everscale network             | https://eri01.main.everos.dev/graphql  https://gra01.main.everos.dev/graphql  https://gra02.main.everos.dev/graphql  https://lim01.main.everos.dev/graphql  https://rbx01.main.everos.dev/graphql | https://eri01.main.everos.dev/  https://gra01.main.everos.dev/  https://gra02.main.everos.dev/  https://lim01.main.everos.dev/  https://rbx01.main.everos.dev/ | wss://eri01.main.everos.dev/graphql    wss://gra01.main.everos.dev/graphql    wss://gra02.main.everos.dev/graphql    wss://lim01.main.everos.dev/graphql    wss://rbx01.main.everos.dev/graphql |
| EVER OS Cloud for Developer network                                | Access to TON Labs Development Network  | https://eri01.net.everos.dev/graphql  https://rbx01.net.everos.dev/graphql  https://gra01.net.everos.dev/graphql                                                                                      | https://eri01.net.everos.dev/  https://rbx01.net.everos.dev/  https://gra01.net.everos.dev/                                                                        | wss://eri01.net.everos.dev/graphql   wss://rbx01.net.everos.dev/graphql    wss://gra01.net.everos.dev/graphql                                                                                       |
| [Evernode Startup Edition](https://github.com/tonlabs/evernode-se) | Access to Evernode SE for local testing | http://localhost/graphql  http://127.0.0.1/graphql  http://0.0.0.0/graphql  (*nix only)                                                                                                             | http://localhost/  http://127.0.0.1/  http://0.0.0.0/                                                                                                              | wss://localhost                                                                                                                                                                                         |

## Connect your application to EVER OS

Find out how to [connect your JS application to EVER OS](https://docs.everos.dev/ever-sdk/guides/installation/configure_sdk).

## Connect TONOS-CLI to EVER OS

Find out how to [connect TONOS-CLI to EVER OS](https://github.com/tonlabs/tonos-cli#21-set-the-network-and-parameter-values).

## Other Clients

If you use another language check the official GraphQL documentation how to connect:

* via [other GraphQL Clients](https://graphql.org/code/)
* via [HTTP requests](https://graphql.org/learn/serving-over-http/)
* via websocket protocol [https://github.com/apollographql/subscriptions-transport-ws/blob/master/PROTOCOL.md](https://github.com/apollographql/subscriptions-transport-ws/blob/master/PROTOCOL.md)

In the next section find out how to work with GraphQL Web playground and easily explore blockchain data with it.

> The documentation in Everscale repository is a community effort. Therefore, everyone can contribute with proposals for new topics, suggest new content elements, participate in editing, and provide ideas that will be of great help for network development. Please be informed that our documentation can be edited via GitHub. It can be found [**here**](https://docs.everscale.network/). 
Please make sure to consult our rules and rewards policy via [**this link**](https://docs.everscale.network/contribute/hot-streams/documentations).  
Also, for any questions that may arise, you can text via this [**Telegram chat**](https://t.me/+C2IpQXWZtCwxYzEy).