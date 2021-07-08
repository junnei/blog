---
layout: default
title: Music Information Retrieval
lang: en
lang-ref: music-information-retrieval
nav_order: 2
has_children: true
permalink: /en/music-information-retrieval
---

# Music Information Retrieval
{: .no_toc }


Music information retrieval (MIR)[[Wiki]](https://en.wikipedia.org/wiki/Music_information_retrieval)<br>is the interdisciplinary science of retrieving information from music.
{: .fs-6 .fw-300 }

Those involved in MIR may have a background in musicology, psychoacoustics, psychology, academic music study, signal processing, informatics, machine learning, optical music recognition, computational intelligence or some combination of these.
{: .fs-5 .fw-300 }


---

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }

1. TOC
{:toc}

</details>


---


# [](#applications)Applications

MIR is being used by businesses and academics to categorize, manipulate and even create music.
On this page, I would like to introduce five applications based on [[MIR Wikipedia]](https://en.wikipedia.org/wiki/Music_information_retrieval).
{: .fs-5 }

## [](#1.1)Music classification

One of the classical MIR research topic is genre classification, which is categorizing music items into one of pre-defined genres such as classical, jazz, rock, etc. Mood classification, artist classification, and music tagging are also popular topics.

## [](#1.2)Recommender systems

Several [recommender systems](https://en.wikipedia.org/wiki/Recommender_system) for music already exist, but surprisingly few are based upon MIR techniques, instead making use of similarity between users or laborious data compilation. [Pandora](https://en.wikipedia.org/wiki/Pandora_Radio), for example, uses experts to tag the music with particular qualities such as "female singer" or "strong bassline". Many other systems find users whose listening history is similar and suggests unheard music to the users from their respective collections. MIR techniques for [similarity in music](https://en.wikipedia.org/wiki/Musical_similarity) are now beginning to form part of such systems.

## [](#1.3)Music source separation and instrument recognition

Music source separation is about separating original signals from a mixture audio signal. Instrument recognition is about identifying the instruments involved in music. Various MIR systems have been developed that can separate music into its component tracks without access to the master copy. In this way e.g. karaoke tracks can be created from normal music tracks, though the process is not yet perfect owing to vocals occupying some of the same frequency space as the other instruments.

## [](#1.4)Automatic music transcription

Automatic [music transcription](https://en.wikipedia.org/wiki/Transcription_(music)) is the process of converting an audio recording into symbolic notation, such as a score or a [MIDI file](https://en.wikipedia.org/wiki/MIDI_file#File_formats). This process involves several audio analysis tasks, which may include multi-pitch detection, [onset detection](https://en.wikipedia.org/wiki/Onset_detection#Onset_detection), duration estimation, instrument identification, and the extraction of harmonic, rhythmic or melodic information. This task becomes more difficult with greater numbers of instruments and a greater [polyphony level](https://en.wikipedia.org/wiki/Polyphony_and_monophony_in_instruments)

## [](#1.5)Music generation

The [automatic generation of music](https://en.wikipedia.org/wiki/Automatic_generation_of_music) is a goal held by many MIR researchers. Attempts have been made with limited success in terms of human appreciation of the results.

---

# [](#methods)Methods used


As mentioned above, I would like to introduce three methods according to [[MIR Wikipedia]](https://en.wikipedia.org/wiki/Music_information_retrieval).

## [](#2.1)Data source

[Scores](https://en.wikipedia.org/wiki/Sheet_music) give a clear and logical description of music from which to work, but access to sheet music, whether digital or otherwise, is often impractical. [MIDI](https://en.wikipedia.org/wiki/MIDI) music has also been used for similar reasons, but some data is lost in the conversion to MIDI from any other format, unless the music was written with the MIDI standards in mind, which is rare. Digital audio formats such as [WAV](https://en.wikipedia.org/wiki/WAV), [mp3](https://en.wikipedia.org/wiki/Mp3), and [ogg](https://en.wikipedia.org/wiki/Ogg) are used when the audio itself is part of the analysis. Lossy formats such as mp3 and ogg work well with the human ear but may be missing crucial data for study. Additionally some encodings create artifacts which could be misleading to any automatic analyser. Despite this the ubiquity of the mp3 has meant much research in the field involves these as the source material. Increasingly, metadata mined from the web is incorporated in MIR for a more rounded understanding of the music within its cultural context, and this recently consists of analysis of [social tags](https://en.wikipedia.org/wiki/Social_tagging) for music.

## [](#2.2)Feature representation

Analysis can often require some summarising, and for music (as with many other forms of data) this is achieved by [feature extraction](https://en.wikipedia.org/wiki/Feature_extraction), especially when the audio content itself is analysed and machine learning is to be applied. The purpose is to reduce the sheer quantity of data down to a manageable set of values so that learning can be performed within a reasonable time-frame. One common feature extracted is the [Mel-Frequency Cepstral Coefficient](https://en.wikipedia.org/wiki/Mel-frequency_cepstral_coefficient) (MFCC) which is a measure of the [timbre](https://en.wikipedia.org/wiki/Timbre) of a piece of music. Other features may be employed to represent the [key](https://en.wikipedia.org/wiki/Tonality#Computational_methods_to_determine_the_key), chords, harmonies, [melody](https://en.wikipedia.org/wiki/Melody), main [pitch](https://en.wikipedia.org/wiki/Pitch_(music)), [beats per minute](https://en.wikipedia.org/wiki/Beats_per_minute) or rhythm in the piece. There are a number of available audio feature extraction tools [Available here](https://www.ntnu.edu/documents/1001201110/1266017954/DAFx-15_submission_43_v2.pdf)

## [](#2.3)Statistics and machine learning
* Computational methods for classification, clustering, and modelling — musical feature extraction for mono- and [polyphonic](https://en.wikipedia.org/wiki/Polyphonic) music, similarity and [pattern matching](https://en.wikipedia.org/wiki/Pattern_matching), retrieval
* Formal methods and databases — applications of automated [music identification](https://en.wikipedia.org/wiki/Music_identification) and recognition, such as [score following](https://en.wikipedia.org/wiki/Score_following), automatic accompaniment, routing and filtering for music and music queries, query languages, standards and other metadata or protocols for music information handling and [retrieval](https://en.wikipedia.org/wiki/Information_retrieval), [multi-agent systems](https://en.wikipedia.org/wiki/Multi-agent_system), distributed search)
* Software for music information retrieval — [Semantic Web](https://en.wikipedia.org/wiki/Semantic_Web) and musical digital objects, intelligent agents, collaborative software, web-based search and semantic retrieval, [query by humming](https://en.wikipedia.org/wiki/Query_by_humming) / [Search by sound](https://en.wikipedia.org/wiki/Search_by_sound), [acoustic fingerprinting](https://en.wikipedia.org/wiki/Acoustic_fingerprinting)
* Music analysis and knowledge representation — automatic summarization, citing, excerpting, downgrading, transformation, formal models of music, digital scores and representations, music indexing and [metadata](https://en.wikipedia.org/wiki/Metadata).