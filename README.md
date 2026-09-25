## Sujeewa Mihindupura

[![Email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:mihindupurasujeewa2023@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/sujeewamihindupura)

I read Pali and Sanskrit, and I build tools for the texts I read.

That combination is rarer than it sounds. Plenty of people build retrieval
systems; plenty of people read the Pali canon. The overlap is where the
interesting problems are — because a system that cannot tell a canonical verse
from a fifth-century gloss on it is not simplifying the tradition, it is
quietly rewriting it.

---

### Dhammapada RAG

A retrieval-augmented answering system over the Dhammapada and Buddhaghosa's
commentary, built so that a commentarial gloss is never presented as the plain
sense of a verse.

**[github.com/mihinbuilds/dhammapada-rag](https://github.com/mihinbuilds/dhammapada-rag)**

423 verses · 305 commentarial stories · four separately attributed layers ·
hybrid retrieval with grammar-constrained citation · an evaluation suite with
single-factor ablations and bootstrap confidence intervals.

Ask it what the Buddha asked Kisā Gotamī to bring him and it answers *a mustard
seed from a house that has never seen death* — tagged `commentary`, not
`verse`, because Dhp 114 says nothing about mustard seeds. That distinction is
the whole system.

**Some of what building it turned up:**

- A default context-window size silently deleted the entire commentary layer
  while every automated check reported the system healthy. A second,
  independent truncation removed most of each long narrative from the index.
  Both produced fluent, correctly cited, schema-valid output.
- Prompt instructions barely move structural behaviour. Rearranging the context
  to mirror the taxonomy moves it moderately. Encoding it in the decoding
  grammar is deterministic. Measured at each tier.
- Two of four retrieval components show no measurable effect once ablated
  properly. Reported as null results rather than left out.
- Four documented cases where a claim carried the correct layer tag, a
  resolvable citation, and false content — the failure class that citation
  checking cannot reach.

---

### How I work

I direct the engineering with AI agents and supply the judgment they cannot:
which edition to trust, whether a gloss has been read correctly, and where the
seam between text and commentary actually falls.

The project has a layer called `alignment` because *"story 1.3 explains
Dhp 3–4"* is true of neither the verse nor the commentary — it is a modern
editorial fact, and filing it under `commentary` would attribute to Buddhaghosa
a claim he never made. Nothing in the tooling could have decided that.

I am learning to write the Python myself rather than only read it.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)

---

### Currently

[one line — what you're working on or reading]

More tools for classical texts are in progress. Open to collaboration on
computational work with the Pali canon, and to conversations about retrieval
systems where provenance actually matters.
