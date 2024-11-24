### [Bitsnap](https://bitsnap.io) Integrations

[Bitsnap](https://bitsnap.io) integrates with the vast majority of modern services to acquire and process operational data, extract metrics, classify and validate KPI's.

## IN DEVELOPMENT

NOT READY FOR PRODUCTION USE.

### Industry Specific integrations

 - [Informational Technologies]()
 - [Consulting]()
 - [Education]()
 - [Healthcare]()
 - [Hospitality]()
 - [Rental]()
 - [Logistics]()

### Accounting Services

- [Chargebee](https://github.com/bitsnap/chargebee-api-client) 
- [Freshbooks](https://github.com/bitsnap/freshbooks-api-client)
- [Myob](https://github.com/bitsnap/myob-api-client)
- [Paypal](https://github.com/bitsnap/paypal-api-client)
- [QBO](https://github.com/bitsnap/qbo-api-client)
- [Stripe](https://github.com/bitsnap/stripe-api-client)
- [Wave](https://github.com/bitsnap/wave-api-client)
- [Xero](https://github.com/bitsnap/xero-api-client)
- [Zoho Books](https://github.com/bitsnap/zohobooks-api-client)

### CRM Services

 - [Active Campaign](https://github.com/bitsnap/activecampaign-api-client) 
 - [Engagebay](https://github.com/bitsnap/engagebay-api-client)
 - [Freshdesk](https://github.com/bitsnap/freshdesk-api-client)
 - [Gainsight](https://github.com/bitsnap/gainsight-api-client)
 - [Highrise](https://github.com/bitsnap/highrise-api-client)
 - [Hubspot](https://github.com/bitsnap/hubspot-api-client)
 - [Insightly](https://github.com/bitsnap/insightly-api-client)
 - [Nimble](https://github.com/bitsnap/nimble-api-client)
 - [Pipedrive](https://github.com/bitsnap/pipedrive-api-client)
 - [Salesforce](https://github.com/bitsnap/salesforce-api-client)
 - [Zoho CRM](https://github.com/bitsnap/zohocrm-api-client)

### Customer Feedback Services

 - [Bamboo HR](https://github.com/bitsnap/bamboohr-api-client)
 - [Customerio](https://github.com/bitsnap/customerio-api-client)
 - [Deel](https://github.com/bitsnap/deel-api-client)
 - [Fullstory](https://github.com/bitsnap/fullstory-api-client)
 - [Gatherup](https://github.com/bitsnap/gatherup-api-client)
 - [Prosperstack](https://github.com/bitsnap/prosperstack-api-client)
 - [Sage HR](https://github.com/bitsnap/sagehr-api-client)
 - [Survey Monkey](https://github.com/bitsnap/surveymonkey-api-client)
 - [Workday](https://github.com/bitsnap/workday-api-client)

### HR Payroll Services

 - [Bamboo HR](https://github.com/bitsnap/bamboohr-api-client)
 - [Deel](https://github.com/bitsnap/deel-api-client)
 - [Sage HR](https://github.com/bitsnap/sagehr-api-client)
 - [Workday](https://github.com/bitsnap/workday-api-client)

### Inventory Management Services

 - [Assetpanda](https://github.com/bitsnap/assetpanda-api-client)
 - [Fishbowl](https://github.com/bitsnap/fishbowl-api-client)
 - [Freshservice](https://github.com/bitsnap/freshservice-api-client)
 - [Lightspeed](https://github.com/bitsnap/lightspeed-api-client)
 - [Ship Station](https://github.com/bitsnap/shipstation-api-client)
 - [Upkeep](https://github.com/bitsnap/upkeep-api-client)

### Management Services

 - [Activetrak](https://github.com/bitsnap/activetrak-api-client)
 - [Aha](https://github.com/bitsnap/aha-api-client)
 - [Asana](https://github.com/bitsnap/asana-api-client)
 - [ClickUP](https://github.com/bitsnap/clickup-api-client)
 - [Jira](https://github.com/bitsnap/jira-api-client)
 - [Linear](https://github.com/bitsnap/linear-api-client)
 - [Podio](https://github.com/bitsnap/podio-api-client)
 - [Process Street](https://github.com/bitsnap/processt-api-client)
 - [Teamwork](https://github.com/bitsnap/teamwork-api-client)
 - [Wrike](https://github.com/bitsnap/wrike-api-client)

### Repository Services

 - [Bitbucket](https://github.com/bitsnap/bitbucket-api-client)
 - [Github](https://github.com/bitsnap/github-api-client)
 - [Gitlab](https://github.com/bitsnap/gitlab-api-client)

### Time Tracking Services

 - [Clockify](https://github.com/bitsnap/clockify-api-client)
 - [Harvest](https://github.com/bitsnap/harvest-api-client)
 - [Hubstaff](https://github.com/bitsnap/hubstaff-api-client)
 - [TimelyApp](https://github.com/bitsnap/timelyapp-api-client)
 - [Toggl](https://github.com/bitsnap/toggl-api-client)

### Usage

```go
package main 

import (
  "time"
)

func main() {

}

```

### Development

Install [asdf](https://asdf-vm.com/guide/getting-started.html) with all the dependencies

```bash
git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.14.0
# Add the following to ~/.bashrc:
echo '. "$HOME/.asdf/asdf.sh"' >> ~/.bashrc
# Completions must be configured by adding the following to your .bashrc:
echo '. "$HOME/.asdf/completions/asdf.bash"' >> ~/.bashrc
```

```bash
# install asdf

asdf plugin add golang
asdf plugin add golangci-lint 
asdf plugin add ko
asdf plugin add goreleaser

go install golang.org/x/tools/cmd/goimports@latest
go install mvdan.cc/gofumpt@latest
go install github.com/onsi/ginkgo/v2/ginkgo@latest
```

### Code generation

```bash
# will scrape the existing API documentation pages and emit the respective API client methods
# enums and models validation, where applicable

go generate ./...
```

### Testing

```bash
ginkgo run ./...
```

### TODO
- [ ] provide [Apache Flink](https://flink.apache.org/) [JNI source](https://nightlies.apache.org/flink/flink-docs-master/docs/dev/datastream/sources/) binding
- [ ] provide [Argo Events](https://argoproj.github.io/argo-events/) source binding
- [ ] benchmarks

## License

[Bitsnap Integrations](https://www.bitsnap.io/integrations) golang package is licensed under the terms of [MIT License](LICENSE).