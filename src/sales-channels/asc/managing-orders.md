---
title: Manage Orders and Fulfillment
---


Order information received from Amazon Seller Central shows in the _Recent Orders_ section of the [store dashboard]({% link sales-channels/asc/amazon-store-dashboard.md %}).

![]({% link sales-channels/asc/assets/amazon-recent-orders-imported.png %}){: .zoom}
_Recent Orders_

## With Order Import Enabled

After [store integration]({% link sales-channels/asc/store-integration.md %}), [**Import Amazon Orders**]({% link sales-channels/asc/order-settings.md %}#configure-order-settings) is `Enabled` by default. This means that corresponding Magento orders are created for your Amazon orders and can be managed in the [Magento Orders]({% link sales/orders.md %}) workflow.

{:.bs-callout .bs-callout-info}
Regardless of your order import settings, Amazon orders that existed in your Amazon Seller Central account prior to your [store integration]({% link sales-channels/asc/store-integration.md %}) will not import.

New orders created in Amazon will import into Magento, but not immediately. Amazon assigns a `Pending` status to new orders. After Amazon verifies the order and the payment method, the order status is changed to `Unshipped`. This status change by Amazon triggers the order import into Magento. When imported, the order information appears in the _Recent Orders_ section of the store dashboard, and Magento creates a corresponding order.

Imported Amazon orders can be managed in the [Magento Orders]({% link sales/orders.md %}) and workflow, just like your other Magento stores. Click the Amazon order number shown in the _Order Number_ column to open the order in the [Magento order process]({% link sales/order-processing.md %}#order-view-descriptions).

## With Order Import Disabled

If you do not want to import and manage your your Amazon orders in Magento, you can change the [**Import Amazon Orders**]({% link sales-channels/asc/order-settings.md %}#configure-order-settings) setting to `Disabled`. This means that when new orders are received from Amazon, corresponding Magento orders are created.

When disabled, order information received from Amazon appears in the _Recent Orders_ section of the store dashboard. This order information is view only, and you must manage these orders in Amazon Seller Central. Click the Amazon order number shown in the _Order Number_ column to open the order details in Amazon Seller Central.

## View your recent Amazon order information

1. Click **View Store** on a store card.

1. View your orders in the _Recent Orders_ section.

1. To view order details or manage an order, click the Amazon order number in the _Order Number_ column.

    - If order import is enabled in your [Order Settings]({% link sales-channels/asc/order-settings.md %}), clicking the order number link will open the order in the [Magento Orders]({% link sales/orders.md %}) workflow.
    - If order import is disabled in your [Order Settings]({% link sales-channels/asc/order-settings.md %}), clicking the order number link will open the order details in Amazon Seller Central.

See [Common Order Processing Tasks]({% link sales-channels/asc/common-order-processing.md %})

{% include amazon-workspace-controls.md %}

### Default Columns

|Column|Description|
|---|---|
|Purchase Date|The date of the purchase as received from Amazon Seller Central.|
|Order Number|The order number generated by your Amazon Central Seller account. Click the link to view order details and fulfillment information. |
|Status|The status of the order. Options: Pending / Unshipped / Shipped / Canceled / Completed / Partially Shipped |
|Buyer's Name|The name of the person who placed the order as received from Amazon Seller Central.|
|Grand Total|The total dollar value of the order as received from Amazon Seller Central.|
