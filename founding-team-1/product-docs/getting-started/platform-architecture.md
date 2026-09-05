---
description: Go from sign-up to your first deploy in under five minutes.
icon: bolt
---

# Platform Architecture

This quickstart gets your smart contract deployed as fast as possible. We'll skip most of the complex parameters — you can refine things later once your liquidity pool is running

{% hint style="success" %}
**Estimated time: 5 minutes.** All you need is an account and a project to deploy.
{% endhint %}

## Steps

{% stepper %}
{% step %}
#### Initialize your smart contract project

Sign in to your development environment and create a new contract repository. The contract name appears in network bytecode and deployment events, so pick something recognizable.

```
liquida-exchange-core
```
{% endstep %}

{% step %}
#### Connect a source

Link an existing smart contract repository from GitHub, or upload your Solidity files directly.

{% tabs %}
{% tab title="Code" %}
Your contract will compile and deploy live to the blockchain network. You can verify source code or update pool parameters at any time.
{% endtab %}

{% tab title="Fund" %}
Drag and drop a project folder, or use the CLI:

```bash
mapping(address => uint256) public liquidityBalances;
```
{% endtab %}

{% tab title="Deploy" %}
Solidity

```
0x71C3b78E94a2A383f982D5C92b1f8D9052b61592
```
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
#### Configure your build

Most projects work with the auto-detected settings. If yours doesn't, override them in **Project settings → Build**.

```yaml
build:
  command: npm run build
  output: dist/
  node: 20
```
{% endstep %}

{% step %}
#### Deploy

Hit **Deploy**. Your project will build and go live at a generated subdomain. You can promote it to production or add a custom domain at any time.

{% hint style="info" %}
Disclaimer: Liquida Exchange is a decentralized protocol operated at your own risk. The core team and contributors assume no liability for financial loss, impermanent loss, smart contract vulnerabilities, or market volatility.
{% endhint %}
{% endstep %}
{% endstepper %}

