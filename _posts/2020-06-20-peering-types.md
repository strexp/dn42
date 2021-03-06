---
date: 2020-06-20
title: Peering Types / 对等互联类型
categories: IP-Services
description: Our Peering Types in DN42 / 我们在 DN42 中的对等互联类型
type: Document
---

## Default / 默认

StrExp considers all requests by default to be of the Transit type unless otherwise specified, and believes that this will help improve the decentralization level of the entire network.

StrExp 默认认为所有的请求，除非特别指定，均为 Transit 类型，并相信这样有助于提升整个网络的去中心化水平。

---

## Transit

- We will receive any legal routes
- We will send all known legal routes

- 我们将接收任何发来的合法路由
- 我们将发送已知的所有合法路由

---

## Peer

- We will receive routes that belong to the other peer's network
- We will send only routes that belong to our own network

- 我们将接收仅属于对方网络的路由
- 我们将发送仅属于己方网络的路由

---

## Downstream

- We will receive routes that belong to the other peer's network
- We will send all known legal routes

- 我们将接收仅属于对方网络的路由
- 我们将发送已知的所有合法路由

---

## Upstream

- We will receive any legal routes
- We will send routes that belong to our own network
- We will send routes from Downstream network

- 我们将接收任何发来的合法路由
- 我们将发送仅属于己方网络的路由
- 我们将发送来自 Downstream 网络的路由
