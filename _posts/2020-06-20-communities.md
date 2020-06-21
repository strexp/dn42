---
date: 2020-06-20
title: Supported BGP Communities / 支持的 BGP 社区
categories: IP-Services
description: Our BGP communities in DN42 / 我们在 DN42 中的 BGP 社区
type: Document
---

We adopted the BGP community settings recommended in the DN42 Wiki. At the same time, we recommend that other networks deploy similar strategies.

我们采用了 DN42 Wiki 中推荐的 BGP 社区设置。同时，我们建议其他网络部署类似的策略。

---

## Continent / 大洲

- (64511, 41) :: Europe / 欧洲
- (64511, 42) :: North America-E / 北美东部
- (64511, 43) :: North America-C / 北美中部
- (64511, 44) :: North America-W / 北美西部
- (64511, 45) :: Central America / 中美洲
- (64511, 46) :: South America-E / 南美洲东部
- (64511, 47) :: South America-W / 南美洲西部
- (64511, 48) :: Africa-N (above Sahara) / 撒哈拉以北非洲
- (64511, 49) :: Africa-S (below Sahara) / 撒哈拉以南非洲
- (64511, 50) :: Asia-S (IN,PK,BD) / 南亚
- (64511, 51) :: Asia-SE (TH,SG,PH,ID,MY) / 东南亚
- (64511, 52) :: Asia-E (JP,CN,KR) / 东亚
- (64511, 53) :: Pacific / 太平洋

---

## Bandwidth / 带宽

- (64511, 21) :: bw >= 0.1mbit
- (64511, 22) :: bw >= 1mbit
- (64511, 23) :: bw >= 10mbit
- (64511, 24) :: bw >= 100mbit
- (64511, 25) :: bw >= 1000mbit
- (64511, 2x) :: bw >= 10^(x-2) mbit

bw = min(up,down) (for asymmetric connections) / (对于非对称带宽链路)

---

## Latency / 延迟

- (64511, 1) :: (0, 2.7ms]
- (64511, 2) :: (2.7ms, 7.3ms]
- (64511, 3) :: (7.3ms, 20ms]
- (64511, 4) :: (20ms, 55ms]
- (64511, 5) :: (55ms, 148ms]
- (64511, 6) :: (148ms, 403ms]
- (64511, 7) :: (403ms, 1097ms]
- (64511, 8) :: (1097ms, 2981ms]
- (64511, 9) :: 2981ms
- (64511, x) :: [exp(x-1), exp(x)] ms (for x < 10)

---

## Tunnel Type / 隧道类型

- (64511, 31) :: not encrypted / 未加密
(64511, 32) :: encrypted with unsafe vpn solution / 使用非安全 VPN 加密
(64511, 33) :: encrypted with safe vpn solution (but no PFS - the usual OpenVPN p2p configuration falls in this category) / 使用安全的 VPN 解决方案加密（但没有 PFS - 常规的 OpenVPN p2p 配置属于此类）
(64511, 34) :: encrypted with safe vpn solution with PFS (Perfect Forward Secrecy) / 使用安全的 VPN 解决方案和 PFS（完全前向保密）进行加密
(64511, 35) :: physical connection / 物理链路

---

## Local Pref

