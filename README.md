Netuitive Windows Agent
========================

The Netuitive Windows Agent leverages CollectdWin to collect, aggregate, and publish windows performance counters and attributes to Netuitive. It is designed to expose crucial metrics from your Windows machines and display them in a meaningful way in [Virtana](https://www.virtana.com/products/cloudwisdom/). 

See the [Netuitive Windows agent docs](https://docs.virtana.com/en/windows-agent.html) or the [wiki](../../wiki) for more information, or contact Netuitive support at [cloudwisdom.support@virtana.com](mailto:cloudwisdom.support@virtana.com).

Changes to CollectdWin
-----------------------

The base functionality of CollectdWin remains in our fork: exposing windows performance counters for collection and monitoring. The Netuitive Windows Agent diverges from CollectdWin by extending the collection to non-numeric values such as attributes, events, and relationships. Netuitive created plugins to read Windows events and attributes as well as plugins to write to [Virtana](https://www.virtana.com/products/cloudwisdom/) and [StatsD](https://github.com/etsy/statsd). Netuitive also changed the underlying framework to support collection and representation of elements of different types and metrics from remote sources.

