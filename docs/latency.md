# API Latency

As you may have noticed, the API is quite slow and it's done on purpose. 

We are using the [Otoroshi Defer Responses plugin](https://maif.github.io/otoroshi/manual/plugins/built-in-plugins.html#otoroshi.next.plugins.NgDeferPlugin) 
to introduce artifical latency in order to demonstrate how [react-query](https://tanstack.com/query/latest/docs/framework/react/overview) works

By default, the latency is setup to 800 ms.