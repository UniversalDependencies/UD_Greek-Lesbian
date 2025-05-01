# Summary

A Universal Dependencies (UD) treebank for the dialect of Lesbos, a low-resource living Northern variety of Modern Greek. The treebank currently contains 270 sentences with manual annotations following the Universal Dependencies framework, representing the first UD treebank for a Northern Modern Greek dialect.

# Introduction

The Lesbos dialect belongs to the Northern Modern Greek dialect group, characterized by distinctive phonological features collectively known as "Northern vocalism." These features include:

* Raising of unstressed mid vowels /e/ and /o/ into [i] and [u], respectively (e.g., πιδί [piˈði] instead of SMG παιδί [peˈði] 'child', κάτου [ˈkatu] instead of SMG κάτω [ˈkato] 'down')

* Deletion of unstressed high vowels /i/, /u/ (e.g., φίδ [ˈfið] instead of SMG φίδι [ˈfiði] 'snake', βνό [ˈvno] instead of SMG βουνό [vuˈno] 'mountain')

These features significantly distinguish the dialect of Lesbos from Southern dialects, including Standard Modern Greek (SMG). The dialect has been historically shaped by extensive contact with Italo-Romance (particularly Venetian) during 1355-1462 and Turkish during the Ottoman period (1462-1912), resulting in numerous loanwords and morphological elements. Unlike most Modern Greek dialects, Lesbian remains vital today, serving as the primary means of communication throughout the island.

This treebank represents the first Universal Dependencies resource for a Northern Modern Greek dialect.

## Annotation Process

The treebank follows the UD annotation guidelines established for UD_Greek-GUD, complemented by grammatical descriptions and dialect dictionaries. Key annotation features include:

### Tokenization

* Unlike GUD's approach of pre-tokenizing contracted forms, the Lesbian treebank maintains merged word sequences as written in the original sources and treats them as multi-word tokens. In this line, adposition-determiner contractions are segmented as multi-word tokens (e.g., στο [sto] 'in/to the' is tokenized as two syntactic words, σ [s] 'in/to' and το [to] 'the')

* Clitics frequently attached to verbs in written dialectal texts are handled as multi-word tokens (e.g., τάμπλιξις [ˈtabliksis] '(you) mixed them up' → τά + μπλιξις)

* Possessive pronouns frequently attached to nouns are similarly treated as multi-word tokens (e.g., πατέρασιτς [paˈterasits] 'her father' → πατέρας + ιτς)

* Erroneously split tokens in the original sources are not merged, but instead linked using the "goeswith" relation following UD guidelines

### Lemmatization

* Words diverging from SMG counterparts are assigned lemma forms that preserve dialectal characteristics

* Apostrophes are eliminated from lemmas to standardize representation across inconsistent source texts

* For inconsistently spelled dialectal features, the dialectologically expected form (with vowel raising and deletion) is consistently used as the lemma

* SMG orthography is applied to lemmas regardless of orthographic errors in source materials

### Special Annotations

* Voicing and euphonic annotations in the MISC column using MSeg|MGloss format to document these phenomena explicitly

* Orthographic standardization integrated with annotations, preserving original dialectal forms in the FORM column while providing standardized forms in the MISC column

* Parallel translations of each sentence in SMG to facilitate comparative research

## Data Sources

The corpus draws from six main sources representing different text types and dialectal variants from across Lesbos. The treebank consists of randomly shuffled sentences coming from these sources:

### Dialectal Dictionaries (example sentences)

* Papanis, D. and Papanis, G. D. (2004). Lexiko tou Agiasotikou Glosikou Idiomatos [Dictionary of the Agiasos Dialect], 3rd improved and expanded edition. Private edition, Mytilene.

* Ralli, A. (2017). Lexiko dialektikis poikilias. Kydonion-Moschonision kai Voreioanatolikis Lesvou [Dictionary of dialectal variety. Kydonies-Moschonisia and Northeastern Lesbos]. Hellenic Foundation for Historical Studies, Athens.

* Anagnostopoulou, M. A. (2021). Thematiko Lexiko tis Lesviakis Dialektou [Thematic Dictionary of the Lesbos Dialect]. Mythos BOOKS, Mytilene.

### Contemporary Lesbian Literature

* Tsokarou-Mitsioni, E. (1998). Palies Istories ap tn Agiasiou [Old Stories from Agiasio], 2nd edition. Private Edition, Mytilene.

* Anagnostou, V. T. (2014). Tsi sta th'ka mas: Komodia sta k'stariot'ka [Tsi sta th'ka mas: Comedy in the K'stariot'ka Dialect], first edition. Estia Technon Skoutarou "T'Apono to Scholio".

* Tsokarou-Mitsioni, E. (2019). Prosfygiá [Refugeehood], first edition. D. Doukas & Sia O.V.E.E.

# Statistics

* Sentences: 270

* Tokens: 3,603


# Acknowledgments

This work has been carried out within the Archimedes Research Unit of the Athena Research Center, Greece. It has been partially supported by project MIS 5154714 of the National Recovery and Resilience Plan Greece 2.0, funded by the European Union under the NextGenerationEU Program. It also received support from the CA21167 COST action UniDive, funded by COST (European Cooperation in Science and Technology).

# References

* TBA


# Changelog

* 2024-11-15 v2.15
  * Initial release in Universal Dependencies.


<pre>
=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.15
License: CC BY-SA 4.0
Includes text: yes
Genre: grammar-examples, spoken, fiction
Lemmas: manual native
UPOS: manual native
XPOS: not available
Features: manual native
Relations: manual native
Contributors: Bompolas, Stavros; Markantonatou, Stella; Anastasopoulos, Antonios; Stamou, Vivian
Contributing: here
Contact: s.bompolas@athenarc.gr
===============================================================================
</pre>
