## Sujeewa Mihindupura

[![Email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:mihindupurasujeewa2023@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/sujeewamihindupura)

I read Pali and Sanskrit, and I build tools for the texts I read.

A system that cannot tell a canonical verse from a fifth-century gloss on it
is not simplifying the tradition — it is quietly rewriting it.

---

### [Dhammapada RAG →](https://github.com/mihinbuilds/dhammapada-rag)

Retrieval-augmented answering over the Dhammapada and Buddhaghosa's commentary,
built so a commentarial gloss is never presented as the plain sense of a verse.

423 verses · 305 commentarial stories · four separately attributed layers ·
grammar-constrained citation · ablations with confidence intervals.

Ask it what the Buddha asked Kisā Gotamī to bring him and it answers *a mustard
seed from a house that has never seen death* — tagged `commentary`, not
`verse`, because Dhp 114 says nothing about mustard seeds. That distinction is
the whole system.

One thing building it turned up: a default context-window size silently deleted
the entire commentary layer while every automated check reported the system
healthy. The output stayed fluent, cited and schema-valid throughout.

---

### How I work

I direct the engineering with AI agents and supply the judgment they cannot —
which edition to trust, whether a gloss has been read correctly, where the seam
between text and commentary falls. The project has a layer called `alignment`
because *"story 1.3 explains Dhp 3–4"* is true of neither the verse nor the
commentary. Nothing in the tooling could have decided that.

Learning to write the Python myself rather than only read it.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)

---

More tools for classical texts in progress. Open to collaboration on
computational work with the Pali canon.
