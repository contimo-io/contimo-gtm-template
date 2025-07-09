# Conversion Tracking in Contimo with Google Tag Manager

To set up conversion tracking with Contimo using Google Tag Manager (GTM), follow these steps:

1. **Install the Contimo Template**  
   - In GTM, go to the Template Gallery and add the official Contimo tag template to your workspace.

2. **Configure the Contimo Tag for Page Views**  
   - Create a new tag using the Contimo template.
   - Set the **Action** parameter to `Init`.
   - Configure the tag to capture the Contimo Click ID. For example, use a URL variable such as `cntmclid` to store the click ID from the landing page URL.
   - Set the trigger to fire this tag on all page views.

3. **Set Up the Conversion Tag**  
   - Create another tag using the Contimo template.
   - Set the **Action** parameter to `Conversion`.
   - Configure the tag to fire when a conversion event occurs (e.g., after a successful purchase or form submission).
   - You can specify additional parameters, such as the conversion type and transaction revenue, to enable detailed ROAS (Return on Ad Spend) analysis.

**Tip:**  
Make sure the Click ID (`cntmclid`) is consistently passed from the landing page through to the conversion event, so conversions can be accurately attributed.

For more details on macros and parameters, see the [Supported Macros](01-macro.md) and [Conversion Tracking](02-conversion-tracking.md) documentation.