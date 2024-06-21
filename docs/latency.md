# API Latency

As you may have noticed, the API is quite slow and it's done on purpose. 

We are using the [Otoroshi Defer Responses plugin](https://maif.github.io/otoroshi/manual/plugins/built-in-plugins.html#otoroshi.next.plugins.NgDeferPlugin) 
to introduce artifical latency in order to demonstrate how [react-query](https://tanstack.com/query/latest/docs/framework/react/overview) works

By default, the latency is setup to 800 ms.

<div style="width: 100%; display: flex; justify-content: center; align-items: center;">
  <img src="/docs/defer.png" alt="The defer responses plugin" width="1000" height="auto" class="centered-img">
</div>