# OAuth2 Proxy BOSH Release

This is a [BOSH](http://bosh.io/) release for [OAuth2 Proxy](https://github.com/pusher/oauth2_proxy). It is intended to be deployed as a reverse proxy that provides authentication using Providers (Google, GitHub, and others) to validate accounts by email, domain or group.

## Table of Contents

* [Usage](https://github.com/bosh-prometheus/prometheus-boshrelease#usage)
	* [Operations files](https://github.com/bosh-prometheus/prometheus-boshrelease#operations-files)

## Usage

### Operations files

Additional [operations files](http://bosh.io/docs/cli-ops-files.html) are located at the [manifests/operators](https://github.com/Infra-Red/oauth2-proxy-boshrelease/blob/master/manifests/operators) directory. Those files includes an extension for the existing bosh releases.

Please review the op files before deploying them to check the requeriments, dependencies and necessary variables.

| File | Description | BOSH Release |
| ---- | ----------- | ------------ |
| [enable-prometheus-oauth2-proxy.yml](https://github.com/Infra-Red/oauth2-proxy-boshrelease/blob/master/manifests/operators/prometheus/enable-prometheus-oauth2-proxy.yml) | Enables OAuth2 Proxy for Prometheus and Alertmanager | [prometheus-boshrelease](https://github.com/bosh-prometheus/prometheus-boshrelease) |