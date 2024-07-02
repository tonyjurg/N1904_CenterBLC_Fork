<a name="start"></a>
<div class="hidden-content">
<a href="../transcription.md">Transcription</a> | <a href="README.md#start">Features</a> | <a href="../viewtypes.md#start">Viewtypes</a> | <a href="../textformats.md#start">Textformats</a> |  <a href="../syntaxtrees.md#start">Syntaxtrees</a> | <a href="../../tutorial/README.md#start">Tutorial</a> | <a href="../usecases/README.md#start">Usecases</a> | <a href="../about.md#start">About</a>
</div>

# Nestle 1904 GNT - Feature: otext

Feature group | Feature type | Data type | Available for node types | Used by viewtypes
---  | --- | --- | --- | ---
[`Grid`](featuresbygroup.md#grid-features) | [`Config`](featuresbyfeaturetype.md#config-features) | *not applicable* | *not applicable* | [`syntax-view`](../syntax-view.md#start) [`wg-view`](../wg-view.md#start)

## Feature description

Textformatting and corpus segmenting configuration used by the text API. 

## Notes 

This feature does not contain node specific data, but contains information that tells Text-Fabric how to produce text strings for slots and the structure of the corpus.

The defined [text-formating options](../textformats.md#start) for this dataset are:
<pre>
  A.showFormats()
     format               level   template
     lex-orig-plain       word    {lemma}{punctuation}
     lex-translit-plain   word    {lemmatranslit}{punctuation}
     text-orig-full       word    {before}{text}{after}
     text-orig-plain      word    {text}{punctuation}
     text-translit-plain  word    {translit}{punctuation}
     text-unaccent-plain  word    {unaccent}{punctuation}
</pre>

The declaretion of section level by feature otext is used to format the output of functions like [T.sectionFromNode(node)](https://annotation.github.io/text-fabric/tf/cheatsheet.html#sections). In this dataset section structure is the three level book, chapter, and verse division of the material.

## Source description

Defined during creation of the  dataset.

---
##### *Browse all features by [node type](featuresbynodetype.md#start), [data type](featuresbydatatype.md#start), [feature group](featuresbygroup.md#start) or [feature type](featuresbyfeaturetype.md#start).*
