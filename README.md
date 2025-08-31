Workflow Steps

Data Fetching:

Six separate Google Analytics data pulls:
Page Engagement Stats (This Week and Prior Week)
Google Search Results (This Week and Prior Week)
Country Views (This Week and Prior Week)
Data Parsing:

Each data pull is processed using a dedicated parser node to generate a URL-safe string.
Example nodes:
Parse - Get Page Engagement This Week
Parse - Country Views Prior Week
Data Aggregation:

Aggregates parsed data into a structured JSON object using the Aggregate Data node.
Ensures consistency and handles missing or malformed data.
HTML Report Generation:

Creates a formatted HTML report with color-coded tables for each segment:
Engagement Stats: Green
Search Results: Blue
Country Views: Orange
Includes headers and neatly formatted tables for each data set.
Output:

The report can be sent via email using the Gmail API or saved to Google Docs.
Example nodes:
Gmail node for email delivery.
Google Docs node for saving the report as a document.
