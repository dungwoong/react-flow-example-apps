- npm install @xyflow latest or smth like that

Nodes/index.ts
- in nodes, they declare their initial node. In nodetypes, they add custom node type mappings
- default node type has input/output edge, input only has bottom input edge, output has top output edge
- group node type is for grouping: [subgraphs docs](https://reactflow.dev/examples/layout/sub-flows)
- all the node type attributes [here](https://reactflow.dev/api-reference/types/node)

PositionLoggerNode
- you can look at nodeprops to see what's in there
- node data also has props
- I think source is you can drag out from there, target is you can create an edge that leads to there
- all incoming edges will go to the target, all outgoing edges come from the source
- I dunno, we can just read [the handle docs](https://reactflow.dev/api-reference/components/handle) if we want

Edges/index.ts
- you basically declare source, target, type
- there's like animated or whatever...
- [custom edges](https://reactflow.dev/examples/edges/custom-edges)
- you can change defaultEdgeOptions={{ type: "button-edge" }} in Flow.tsx