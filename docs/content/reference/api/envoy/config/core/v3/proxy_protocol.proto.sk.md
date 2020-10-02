
---
title: "proxy_protocol.proto"
weight: 5
---

<!-- Code generated by solo-kit. DO NOT EDIT. -->


### Package: `envoy.config.core.v3` 
#### Types:


- [ProxyProtocolConfig](#proxyprotocolconfig)
- [Version](#version)
  



##### Source File: `envoy/config/core/v3/proxy_protocol.proto`





---
### ProxyProtocolConfig



```yaml
"version": .envoy.config.core.v3.ProxyProtocolConfig.Version

```

| Field | Type | Description | Default |
| ----- | ---- | ----------- |----------- | 
| `version` | [.envoy.config.core.v3.ProxyProtocolConfig.Version](../proxy_protocol.proto.sk/#version) | The PROXY protocol version to use. See https://www.haproxy.org/download/2.1/doc/proxy-protocol.txt for details. |  |




---
### Version



| Name | Description |
| ----- | ----------- | 
| `V1` | PROXY protocol version 1. Human readable format. |
| `V2` | PROXY protocol version 2. Binary format. |





<!-- Start of HubSpot Embed Code -->
<script type="text/javascript" id="hs-script-loader" async defer src="//js.hs-scripts.com/5130874.js"></script>
<!-- End of HubSpot Embed Code -->