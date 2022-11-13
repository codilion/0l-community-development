# 0L Community Development Wallet

## Purpose

With the help of this community wallet, the 0L network community will be developed across all platforms. offers funds for activities that help build, grow, and maintain a vibrant decentralized community, including ambassador programs, guest speakers, premium services used in the community, and similar activities.

## Payment and structure

The details of each payment will be recorded in this repository.

The steward running the community wallet is `Daniyal#9700` on the [0L Discord server](https://discord.gg/0lnetwork)

## Contribution to the wallet

For validators wishing to help fund the community development programs wallet:

1. Add a json file as `community-development.json`

```yaml
{
  "autopay_instructions": [
    {
      "note": "0L Community Development Wallet: https://github.com/codilion/0l-community-development",
      "uid": 0,
      "destination": "fbe8da53c92ceeeb40d8967ec033a0fb",
      "type_of": "PercentOfChange",
      "value": 1,
      "duration_epochs": 1000
    }]
}
```

2. Enable autopay (if not already enabled)
`txs autopay -e`

3. Add guild autopay
`txs autopay-batch -f community-development.json`
