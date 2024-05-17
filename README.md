<p align="center">
  <picture>
    <img alt="Medusa store-analytics logo" src="./docs/store-analytics-logo.PNG">
  </picture>
</p>

<h1 align="center">
  Medusa store-analytics
</h1>

A fork of [@rsc-labs/medusa-store-analytics](https://medusajs.com/plugins/@rsc-labsmedusa-store-analytics/?hl=en-PH)

Medusa "store-analytics" is a plugin which shows analytics data of your store, including orders, sales and other useful information.

### Why?

Knowledge about your store is crucial to take proper action to increase the sales. Analytics data can show various things like what is a most popular region, sales channel or on which day people are buying the most. Every such data may help to find problem and possible solutions. 

## Getting Started

1. Install the package with `yarn add @Jacavena/medusa-store-analytics-custom` or `npm i @Jacavena/medusa-store-analytics-custom`.
2. In `medusa-config.js`, add the plugin to the `plugins` array and set `enableUI`

```js
const plugins = [
  // ... other plugins
  {
    resolve: `@Jacavena/medusa-store-analytics-custom`,
    options: {
      enableUI: true
    }
  }
]
```



## How can I use it?

After installation of plugin, you shall be able to see new option on sidebar. Click `Analytics` and see data about your store.

<p align="center">
  <picture>
    <img alt="Medusa store-analytics-1" src="./docs/medusa-store-analytics-1.PNG">
  </picture>
</p>

**WARNING**:

Depends on the number of your orders, customers and other - it might take a while to load them all if you click wider options like `Last year` or `All time`!

### Configuration

No configuration is needed. Everything is done through UI. You can use such options like:
- set different range for dates
- set different statuses of orders for calculation
- enabling/disabling comparison feature

<p align="center">
  <picture>
    <img alt="Medusa store-analytics-2" src="./docs/medusa-store-analytics-2.PNG">
  </picture>
</p>

<p align="center">
  <picture>
    <img alt="Medusa store-analytics-3" src="./docs/medusa-store-analytics-3.PNG">
  </picture>
</p>

## Supported statistics

### General

| Name | Status |
| --- | --- |
| 4 ranges of dates | :white_check_mark: |
| Comparison across date ranges | :white_check_mark: |
| Filtering by orders' status | :white_check_mark: |

### Orders

| Name | Status |
| --- | --- |
| Orders by time | :white_check_mark: |
| Orders chart | :white_check_mark: |
| Regions popularity | :white_check_mark: |
| Sales channel popularity | :white_check_mark: |
| Orders frequency distribution | :white_check_mark: |
| Payment provider popularity | :white_check_mark: |

### Sales

| Name | Status |
| --- | --- |
| Sales by time | :white_check_mark: |
| Sales by currency code | :white_check_mark: |
| Sales chart | :white_check_mark: |
| Refunds | :white_check_mark: |

### Customers


| Name | Status |
| --- | --- |
| New customers by time | :white_check_mark: |
| Repeat customer rate | :white_check_mark: |
| Customers chart | :white_check_mark: |
| Cumulative customers by time | :white_check_mark: |

### Products

| Name | Status |
| --- | --- |
| Top variants | :white_check_mark: |
| Top returned variants | :white_check_mark: |
| Products sold count | :white_check_mark: |
| Out of the stock variants | BETA |

### Marketing

| Name | Status |
| --- | --- |
| Top discounts | :white_check_mark: |

## License

MIT

## Pro version

The Pro version of medusa-store-analytics expands on the features of the free version with more advanced capabilities such as 
- customizable dashboard - you can create your own dashboard with chosen statistics
- date range picker - choose whatever date range to see statistics exactly for this range
- more than 15 new, advanced statistics - funnels, deep insights about promotions or granular statistics per sales channels.

The Pro version is available under commercial licence - contact labs@rsoftcon.com for more information.

### Hide Pro version tab

We show what advanced features we offer in "Pro version" tab. We try to keep it non-intruisive, but if you feel it differently, you can always hide this tab by setting following environment variable:
`MEDUSA_ADMIN_MEDUSA_STORE_ANALYTICS_HIDE_PRO=true`

After restarting your admin application, you shall have this tab hidden.

---

© 2024 RSC https://rsoftcon.com/
