# SmartcareApps Memory

## Product Entry

- Product name: SmartcareApps.
- Related GUI test flows can enter through the ADC page.
- Asset list related entry: log in to ADC page > Data Visualization menu > left gear icon > Asset Management page > Asset List tab.

## Roles And Accounts

- Common execution user/role for GUI scenario tests: admin user.
- If a specific account, password, tenant, region, or permission boundary is required, confirm it in the current input before generating executable cases.

## Asset Management And Asset List

- Asset List is a tab under the Asset Management page.
- The Asset List page generally contains an asset name input, an asset type selector, a query button, an asset list table, pagination, and total count display.
- Query is the main action for refreshing the asset list by filter conditions.
- Asset List supports querying by asset name, querying by asset type, and querying by the combination of asset name and asset type.
- After query, table data, pagination, and total count should refresh with the current conditions.
- After query, selected or entered filter conditions should remain observable.
- When there is no matched data, the page should show an understandable empty result instead of an abnormal page state.

## Test Data Preparation

- Asset List GUI tests usually require Data Visualization to be deployed.
- Asset List GUI tests usually require SOC data source, DIS data source, and queryable asset object data to be prepared.
- Asset object data should cover data source, component, dashboard, and story line where applicable.

## GUI Assertion Focus

- Tab visibility and selected state.
- Filter area: asset name input, asset type selector, query button.
- Table area: table headers, row data, empty state.
- Pagination area: pagination entry, current page, total count or statistics.
- Query result: result range, pagination total, and filter condition retention.

## Pending Confirmation

- Asset type display values and order may include data source, component, dashboard, and story line; exact wording and order should follow the current requirement or design document.
- The Chinese wording for dashboard may appear as "仪表板" or "仪表盘"; use the current requirement or design document as the source of truth.
- Asset name input length limit may be 256 characters; confirm from the current requirement or design document before generating boundary cases.
- Asset list table headers and association count field wording should follow the current requirement or design document.
