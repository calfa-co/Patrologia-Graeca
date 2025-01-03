# Patrologia-Graeca

The CGPG project (Calfa GRE*g*ORI Patrologia Graeca), led by Jean-Marie Auwers (UCLouvain), aims to OCRize the remaining non-digital versions of the Patrologia Graeca volumes. The project relies on the expertise of [GRE*g*ORI](https://www.gregoriproject.com) and [Calfa](https://calfa.fr).

The project is sponsored by the ASBL *Byzantion*, the Fondation *Sedes Sapientiae*, the Institut *Religions, Spiritualités, Cultures, Sociétés* (RSCS, UCLouvain) and the Centre d'études orientales (CIOL, UCLouvain) and by a generous donor who wishes to remain anonymous. Other sponsors have recently expressed their willingness to support the project.

## Modus operandi

The project implements the creation of specialized OCR models for the automatic reading of heavily damaged Patrologia Graeca fonts and for the extraction of Greek content only. The texts produced are then tagged (lemmatization, POS, and morphology). This Github offers the raw data produced. A proofread version of each text will gradually be offered within the GRE*g*ORI interfaces.

## Works and Authors Dataset

| ID  | Edition File         | Edition URL                                                                                  | Author                  | Author URL                                          | Author Date      | Work Description                                                                                                                                                          | Raw Text | Word Count | Markup TXT | Markup XML | Analysis     |
| --- | -------------------- | -------------------------------------------------------------------------------------------- | ----------------------- | -------------------------------------------------- | ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- | ---------- | ---------- | ---------- | ------------ |
| 71  | PG071_ed.pdf         | [Link](https://books.google.be/books?id=worYAAAAMAAJ&redir_esc=y)                             | Cyril of Alexandria     | [Wikipedia](https://en.wikipedia.org/wiki/Cyril_of_Alexandria) | 4th-5th AD      | *Commentarius in Oseam prophetam, in Joelem prophetam, In Amos prophetam, In Abdiam prophetam, In Jonam prophetam, In Michæam prophetam, In Nahum prophetam, In Habacuc prophetam, In Sophoniam prophetam, In Aggæum prophetam.* | Available | 214,479    | Available  | Available  | Forthcoming  |
| 73  | PG073_ed.pdf         | [Link](http://books.google.com/books?id=ywsNQz1fTewC)                                         | Cyril of Alexandria     | [Wikipedia](https://en.wikipedia.org/wiki/Cyril_of_Alexandria) | 4th-5th AD      | *In Joannis Evangelium*                                                                                                                                                 | Available | 230,336    | Available  | Available  | Forthcoming  |
| 155 | PG155_ed.pdf         | [Link](http://books.google.com/books?id=_McUAAAAQAAJ)                                        | Simeon of Thessalonica  | [Wikipedia](https://en.wikipedia.org/wiki/Symeon_of_Thessalonica) | 13th-14th AD    | *Symeonis Opera*                                                                                                                                                        | Available | 204,352    | Available  | Available  | Forthcoming  |
| 158 | PG158_ed.pdf         | [Link](http://books.google.com/books?id=hBIT95lCqEsC)                                        | Michael Glykas          | [Wikipedia](https://en.wikipedia.org/wiki/Michael_Glykas)       | 13th AD         | *Annales, Epstulae*                                                                                                                                                     | Available | 195,144    | Available  | Available  | Forthcoming  |


## File formats description

- `*_text_raw.txt`: UTF-8 plain text, raw OCR result.
- `*_text_markup.txt`: Inherited from `*_text_raw.txt` file, with text structure markups (volume number, page number of the source PDF file), no hyphenation, empty lines deletion.
- `*_text_markup.xml`: Inherited from `*_text_markup.txt` file, XML file enriched with references (volume number, page number of the source PDF file), canonical and intuitive forms; upcoming versions will feature lexical analysis (lemmatization and POS tagging).

## Ground-truth

A first training dataset has been released on Zenodo in 2022 : [https://zenodo.org/records/7296539](https://zenodo.org/records/7296539).

```latex
@dataset{vidal_gorene_2022_7296539,
  author       = {Vidal-Gorène, Chahan and
                  Kindt, Bastien},
  title        = {Patrologia Graeca (OCR ground truth)},
  month        = nov,
  year         = 2022,
  publisher    = {Zenodo},
  version      = {1.0.0},
  doi          = {10.5281/zenodo.7296539},
  url          = {https://doi.org/10.5281/zenodo.7296539}
}
```

## Bibliography

### Within the scope of the CGPG project

#### About guidelines for transcription and layout analysis

```latex
@article{vidalgorene:hal-03982432,
  TITLE = {{La reconnaissance automatique d'écriture à l'épreuve des langues peu dotées}},
  AUTHOR = {{Vidal-Gorène, Chahan}},
  URL = {https://enc.hal.science/hal-03982432},
  JOURNAL = {{The Programming Historian en français}},
  NUMBER = {5},
  YEAR = {2023},
  DOI = {10.46430/phfr0023},
}
```

```latex
@article{vidalgorene:hal-04565386,
  TITLE = {{Reconhecimento autom{\'a}tico de manuscritos para o teste de idiomas n{\~a}o latinos}},
  AUTHOR = {{Vidal-Gorène, Chahan and Paulino, Joana}},
  URL = {https://hal.science/hal-04565386},
  JOURNAL = {{Programming Historian em portugu{\^e}s}},
  NUMBER = {4},
  YEAR = {2024},
  DOI = {10.46430/phpt0046},
}
```

### Related publications

```latex
@article{kindt2022analyse,
  title={Analyse automatique du grec ancien par r{\'e}seau de neurones. {\'E}valuation sur le corpus De Thessalonica Capta},
  author={Kindt, Bastien and Vidal-Gor{\`e}ne, Chahan and Delle Donne, Saulo},
  journal={Bulletin de l’Acad{\'e}mie Belge pour l’{\'E}tude des Langues Anciennes et Orientales},
  pages={537--562},
  year={2022}
}
```

```latex
@article{kindt2022manuscript,
  title={From Manuscript to Tagged Corpora},
  author={Kindt, Bastien and Vidal-Gor{\`e}ne, Chahan},
  journal={Armeniaca-International Journal of Armenian Studies},
  volume={1},
  pages={73--96},
  year={2022}
}
```