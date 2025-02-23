# Overview

EMQX Cloud Bills are based on the consumption of deployments and other services within your account. This includes the total deployments and services created by both root account and subaccounts.

You can either pay as you go in an hourly basis or make an annual prepaid purchase. For the plan pricing details, see the [Product Pricing](../price/pricing.md) page.

## Billing cycle

Billing for each EMQX Cloud deployment and service accrues at hourly intervals. Any usage that is less than an hour is billed for the full hour. All billing computations are conducted in Coordinated Universal Time (UTC). 

Billing accrues hourly, with a monthly-in-arrears bill cycle. If you deprovision deployments that have accrued billed usage during the current month, billing will no longer accrue for these deployments, but billed usage accrued so far in the bill cycle will appear on your next bill and invoice.

Billing occurs on the first day of the month for the previous month. For example, if you start a deployment on September 15, you’re billed on October 1 for your usage from September 15-30.


## Monthly Bills

![month bill](./_assets/monthly_bill.png)

The Monthly Bill card will show the total amount of usage. You can change the billing period in the right top corner of the card. You can select billing period up to the last 12 months. 

:::tip
The estimated total amount of the current month excludes taxes. The total amount will be calculated in the beginning of next month, which will include all the taxes and other charges.
:::

- Click **Bill** to navigate to the Bills page to see all the Bills from all time.
- Click **Charges by service** to navigate to the Charges by service page to view the details about all the charges generated by deployments and services.

### Available Credits

**Avaiable Credits** in the bottom right corner of the card shows the credits can be consumed that is held by the prepaid users. 

For those who do not have a credit card or choose other payment methods, Available Credits is the balance for the prepiad payment. 

- The bill is issued monthly. You can check the details in the Bills page.
- The tax of the bills will be calculated according the information of you submit to the sales.
- If the Available Credits is insufficient for the coming bill, the system will deduct all the remain Available Credits. The sales may contact you for further affairs.


## Add or Update a Payment Method

See [Billing Information](./billing_information.md) for more details.

## Cost Visualization

### Date-to-Month Usage Chart

![month bill](./_assets/trend.png)

On the Billing Overview page, a Usage chart displays the costs incurred by your account usage over the last 21 days or last 24 months.

## Declined or Late Payment
<table>
   <tr>
      <th>TIMELINE</th>
      <th>ACTION</th>
   </tr>
   <tr>
      <td>Initial declined payment</td>
      <td>We’ll retry charge every 24 hours. During this period, update your payment method to successfully process your payment.</td>
   </tr>
   <tr>
   	  <td>3 days later</td>
   	  <td>All the deployments and services are suspended. Update your payment method to successfully process your payment and enable your services.</td>
   </tr>
   <tr>
   	  <td>5 days later</td>
   	  <td>All the deployments and services will be deleted. Contact cloud-support@emqx.io to get further help.</td>
   </tr>
</table>

## Retry a Failed Payment

If there is an overdue bill, in the top of the Billing Overview page, you will find a message alert. Click "TRY HERE TO PAY THE OVERDUE BILL(s) MANUALLY." to view the overdue bill in Bills page.

View the payment method displayed in the Payment Method card. If this method appears incorrect, click **Change info** in that card.

Click the **Overdue** or **the card icon**, check the failed payment in that month and retry the payment.

![overdue](./_assets/overdue.png)

If the payment is failed again, please contact your card issuer and ask for more information about the declined payment.
