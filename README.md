# Preparing your Claude Style for Rill

To use the DataExplorer style in your Claude Desktop, you need to edit the Explore link examples to suit your project.

1. Edit the Style
2. In Claude Desktop, click on the "Search and Tools" icon below the chat input
3. Click "Create and Edit Styles"
4. Click "Create custom style"
5. Click "Add writing style"
6. Select "Paste text content"
7. Copy and paste the contents of your updated DataExplorer.md file


## Editing the Style

1. Edit the BASE_URL to match your project in Rill Cloud
2. Create an METRICS_EXPLORE_SLUG for each Explore in the project
3. Use Rill to create an entire URL for each example
4. Copy that URL into the `Link:` using the format below
5. Repeat for each example:
    - Multiple metrics and dimensions
    - Individual metric
    - Individual dimension 

## Example

**Example: Link for an explore with multiple metrics and dimensions**
- Description: A link to an online dashboard from Rill. Contains all selected metrics in the report, all dimensions used in the report, and up to 1-3 additional dimensions. Time range includes the range used as the focus of the report, plus a comparison period for enriched visualization. It is in markdown format, and has a link that describes the purpose of the link.
- Format: Markdown
- BASE_URL: `https://ui.rilldata.com/demo/rill-openrtb-prog-ads/explore/`
- METRICS_EXPLORE_SLUG for bids_metrics: `bids_explore`
- METRICS_EXPLORE_SLUG for auctions_metrics: `auctions_explore`
- Link : [<BASE_URL>/<METRICS_EXPLORE_SLUG>?tr=2025-05-17T23%3A00%3A00.000Z%2C2025-05-19T23%3A00%3A00.000Z&tz=Europe%2FLondon&compare_tr=rill-PP&measures=overall_spend%2Ctotal_bids%2Cwin_rate%2Cvideo_completes%2Cavg_bid_floor&dims=advertiser_name%2Csites_domain%2Capp_site_name%2Cdevice_type%2Ccreative_type%2Cpub_name](Explore change in advertising bids due to composition of advertisers)