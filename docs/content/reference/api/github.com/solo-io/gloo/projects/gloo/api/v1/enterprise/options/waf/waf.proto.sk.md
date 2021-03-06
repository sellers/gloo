
---
title: "waf.proto"
weight: 5
---

<!-- Code generated by solo-kit. DO NOT EDIT. -->


### Package: `waf.options.gloo.solo.io` 
#### Types:


- [Settings](#settings)
- [CoreRuleSet](#coreruleset)
  



##### Source File: [github.com/solo-io/gloo/projects/gloo/api/v1/enterprise/options/waf/waf.proto](https://github.com/solo-io/gloo/blob/master/projects/gloo/api/v1/enterprise/options/waf/waf.proto)





---
### Settings



```yaml
"disabled": bool
"customInterventionMessage": string
"coreRuleSet": .waf.options.gloo.solo.io.CoreRuleSet
"ruleSets": []envoy.config.filter.http.modsecurity.v2.RuleSet
"auditLogging": .envoy.config.filter.http.modsecurity.v2.AuditLogging
"requestHeadersOnly": bool
"responseHeadersOnly": bool

```

| Field | Type | Description | Default |
| ----- | ---- | ----------- |----------- | 
| `disabled` | `bool` | Disable waf on this resource (if omitted defaults to false). If a route/virtual host is configured with WAF, you must explicitly disable its WAF, i.e., it will not inherit the disabled status of its parent. |  |
| `customInterventionMessage` | `string` | Custom massage to display if an intervention occurs. |  |
| `coreRuleSet` | [.waf.options.gloo.solo.io.CoreRuleSet](../waf.proto.sk/#coreruleset) | Add OWASP core rule set if nil will not be added. |  |
| `ruleSets` | [[]envoy.config.filter.http.modsecurity.v2.RuleSet](../../../../../external/envoy/extensions/waf/waf.proto.sk/#ruleset) | Custom rule sets rules to add. |  |
| `auditLogging` | [.envoy.config.filter.http.modsecurity.v2.AuditLogging](../../../../../external/envoy/extensions/waf/waf.proto.sk/#auditlogging) | Audit Log settings. |  |
| `requestHeadersOnly` | `bool` | Only process request headers, not buffering the request body. |  |
| `responseHeadersOnly` | `bool` | Only process response headers, not buffering the response body. |  |




---
### CoreRuleSet



```yaml
"customSettingsString": string
"customSettingsFile": string

```

| Field | Type | Description | Default |
| ----- | ---- | ----------- |----------- | 
| `customSettingsString` | `string` | String representing the core rule set custom config options. Only one of `customSettingsString` or `customSettingsFile` can be set. |  |
| `customSettingsFile` | `string` | String representing the core rule set custom config options. Only one of `customSettingsFile` or `customSettingsString` can be set. |  |





<!-- Start of HubSpot Embed Code -->
<script type="text/javascript" id="hs-script-loader" async defer src="//js.hs-scripts.com/5130874.js"></script>
<!-- End of HubSpot Embed Code -->
