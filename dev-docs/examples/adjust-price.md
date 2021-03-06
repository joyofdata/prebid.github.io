---
layout: example
title: Adjust Bidder Price Example
description: Adjust Bidder Price Example with DFP GPT

top_nav_section: dev_docs
nav_section: quick-start

hide: true

about:
- <strong>Adjust bidder price for real earnings.</strong>
- Integration with DFP's GPT single request asynchronous mode.
- One set of line items for all bidders
- Standard keyword targeting setup (<a href="/dev-docs/publisher-api-reference.html#bidderSettingsDefault">reference</a>).
- Standard price granularity (pbMg see <a href="/dev-docs/publisher-api-reference.html#bidResponse">reference here</a>).


jsfiddle_link: jsfiddle.net/prebid/hn06j4f4/2/embedded/html,result

code_height: 2536
code_lines: 116

pid: 80
---

<!-- jsfiddle.net/prebid/hn06j4f4/embedded/html,result -->

<br>
<br>
<br>
<br>
<br>

<div markdown="1">
#### Line 1 to 58: Set timeout and define ad units

Same setup as in [Basic Example](/dev-docs/examples/basic-example.html). Check the basic example page for more details.

</div>

<br><br><br><br><br><br>
<br><br><br><br><br><br>
<br><br><br><br><br><br>
<br><br><br><br><br><br>
<br><br><br><br><br><br>
<br><br><br><br><br><br>
<br><br><br><br><br><br>
<br><br><br><br><br><br>
<br><br><br><br><br><br>
<br><br><br>

<div markdown="1">
#### Line 62 to 64: Adjust Bid Price

Some bidders return gross prices, instead of the net prices (what the publisher will actually get paid). For example, a publisher’s net price might be 15% below the returned gross price. In this case, the publisher may want to adjust the bidder’s returned price to run a true header bidding auction. Otherwise, this bidder’s gross price will unfairly win over your other demand sources who report the real price.

(AppNexus does return the net price. This is just an example for adjusting bid prices.)

In the example, the AOL bidder will inherit from "standard" adserverTargeting keys (default and not shown), so that you don't have to define the targeting keywords again.

</div>
