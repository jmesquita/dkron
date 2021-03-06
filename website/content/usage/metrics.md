---
title: Metrics
---

Dkron has the ability to send metrics to Statsd for dashboards and historical reporting. It sends job processing metrics and golang, serf metrics too.

## Configuration

Add this in your yaml config file

```yaml
dog_statsd_addr: "localhost:8125"
```

## Metrics

- dkron.agent.event_received.query_execution_done
- dkron.agent.event_received.query_run_job
- dkron.memberlist.gossip
- dkron.memberlist.probeNode
- dkron.memberlist.pushPullNode
- dkron.memberlist.tcp.accept
- dkron.memberlist.tcp.connect
- dkron.memberlist.tcp.sent
- dkron.memberlist.udp.received
- dkron.memberlist.udp.sent
- dkron.rpc.call_execution_done
- dkron.rpc.call_get_job
- dkron.rpc.execution_done
- dkron.rpc.get_job
- dkron.runtime.alloc_bytes
- dkron.runtime.free_count
- dkron.runtime.gc_pause_ns
- dkron.runtime.heap_objects
- dkron.runtime.malloc_count
- dkron.runtime.num_goroutines
- dkron.runtime.sys_bytes
- dkron.runtime.total_gc_pause_ns
- dkron.runtime.total_gc_runs
- dkron.serf.coordinate.adjustment_ms
- dkron.serf.msgs.received
- dkron.serf.msgs.sent
- dkron.serf.queries
- dkron.serf.queries.execution_done
- dkron.serf.queries.run_job
- dkron.serf.query_acks
- dkron.serf.query_responses
- dkron.serf.queue.Event
- dkron.serf.queue.Intent
- dkron.serf.queue.Query

