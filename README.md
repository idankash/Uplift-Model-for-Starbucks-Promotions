# Maximizing Marketing ROI: Building an Uplift Model for Starbucks Promotions

*How machine learning can transform promotional campaigns from cost centers into profit drivers*

---

**Interested in the my work?** You can explore the full blog on my *[Medium](https://medium.com/@idankashtan/maximizing-marketing-roi-building-an-uplift-model-for-starbucks-promotions-40c4d27ef1fc)*.

---

![Not All Discounts Are Equal: Target the right customers, and your marketing becomes an investment, not a cost.](/StartbucksPromotion.png)

## Introduction

In today's competitive retail landscape, businesses spend billions on promotional campaigns, yet many struggle to measure their true effectiveness. The fundamental question isn't just "Did customers who received promotions buy more?" but rather "Would they have bought anyway?" This distinction represents the difference between correlation and causation—a critical gap that uplifts modeling bridges.

This case study demonstrates how advanced data science techniques can optimize promotional targeting for maximum business impact. Using a simulated Starbucks dataset, I developed an uplift model that identifies customers most likely to be positively influenced by promotions, transforming marketing spend from a cost center into a strategic profit driver.

## Project Overview

### The Business Challenge

Starbucks faces a common marketing dilemma: how to maximize the return on promotional investments while minimizing wasted spend. In this experiment, we analyze results from a simulated marketing promotion for a $10 product, where each promotional message costs $0.15 to send.

The dataset contains customer responses across two key dimensions:
- **Promotion flag**: Whether the customer received the promotional offer
- **Purchase flag**: Whether the customer ultimately bought the product
- **Customer features**: Seven abstract behavioral indicators (V1-V7)

### Success Metrics

The model's effectiveness is measured through two critical business metrics:

**Incremental Response Rate (IRR)**: The additional percentage of customers who purchase specifically because of the promotion. This metric isolates the promotional impact by comparing response rates between treated and control groups among targeted customers.

*IRR = Response Rate (Targeted) - Response Rate (Control)*

**Net Incremental Revenue (NIR)**: The total additional profit generated after accounting for promotional costs. This represents the true business value created by the campaign.

*NIR = (Incremental Customers × Product Price) - (Total Promotions Sent × Promotion Cost)*

