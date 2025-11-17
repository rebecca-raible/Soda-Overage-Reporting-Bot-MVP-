# Overage Reporting Bot

### Overview
Streams daily customer dataset consumption data, identifies when a contract quota is breached and sends real-time Slack alerts. Every alert will contain customer info, overage amount and tags the responsible account manager, helping SODA to prioritize upsell opportunities. 

### Features
- Overconsumption detection from CSV
- Slack alerts for customer exceeding dataset limits
- Direct @-mentions of account managers
- Alert fatigue reduction (alerts sent out only for new or increased overages)
- Sample Power BI dashboard summarizing historical trends

### Solution tech architecture
- Python script: reads daily data, tracks overages and updates alert state
- Slack integration: alerts posted in a dedicated channel via Slack Webhook
- Manager mapping: maps customer ID to Slack user ID of employee in charge
- Power BI Dashboard: visualizes trends, KPIs


