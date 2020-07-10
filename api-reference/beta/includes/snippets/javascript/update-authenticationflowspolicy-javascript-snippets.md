---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const authenticationFlowsPolicy = {
  selfServiceSignUp: {
    isEnabled: true
  }
};

let res = await client.api('/policies/authenticationFlowsPolicy')
	.version('beta')
	.update(authenticationFlowsPolicy);

```