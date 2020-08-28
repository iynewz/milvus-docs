一般来说，当 <code>nq</code>（每次查询的向量条数）较小时，用 CPU 查询比较快。只有当 <code>nq</code> 较大（约大于 500）时，用 GPU 查询才会更有优势。

因为在 Milvus 中，每次用 GPU 查询都需要将数据从内存加载到显存。只有当 GPU 查询节省的计算时间能抵消掉数据加载的时间，才能体现出 GPU 查询的优势。