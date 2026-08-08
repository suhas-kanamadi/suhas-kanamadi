## Suhas Kanamadi

Final-year Computer Science student at PES University, Bangalore, focused on
systems programming, distributed systems and applied AI.

I'm drawn to problems where correctness is the hard part rather than throughput — filesystems, distributed pipelines, systems whose failure mode is silent rather than loud. Most of what I build starts as "how does this actually work underneath" and ends as a smaller version of the thing.


---

### Projects

**[OverlayFS-Lite](https://github.com/suhas-kanamadi/OverlayFS-Lite)** &nbsp;·&nbsp; C++17, FUSE

A userspace union filesystem that merges a read-only lower layer and a writable upper layer into one mount point. Implements copy-on-write promotion at `open()` and `.wh.` whiteout markers for deletion over immutable storage — the same mechanics behind Docker's layered images. Built with three others; I worked on the copy-on-write and whiteout layers.

**[resume-ranking-pipeline](https://github.com/suhas-kanamadi/resume-ranking-pipeline)** &nbsp;·&nbsp; Python, FastAPI, Kafka, FAISS

A distributed ATS pipeline — spaCy structured extraction, sentence-transformer embeddings, FAISS retrieval, and a hybrid five-signal ranker, decomposed into independent services. Load testing at 200 concurrent connections surfaced a 2.76 MiB-per-response serialization bottleneck that dominated latency; the fix was bounding result sets at the query layer.

**[Requirement-to-Test-Case Generator](https://github.com/suhas-kanamadi/Requirement-to-Test-Case-Generator)** &nbsp;·&nbsp; Python, RAG, ChromaDB

Generates structured test cases from natural-language requirements using retrieval over a curated knowledge base of test patterns. Includes a direct-LLM baseline and an evaluation harness, because "RAG helped" isn't a claim worth making without something to compare against.

---

### Elsewhere

[LinkedIn](https://linkedin.com/in/suhas-kanamadi-804b752b9) &nbsp;·&nbsp; kanamadi.suhas@gmail.com
