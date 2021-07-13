---
layout: default
title: Music Information Retrieval
lang: kr
lang-ref: music-information-retrieval
nav_order: 2
has_children: true
permalink: /kr/music-information-retrieval
---

# Music Information Retrieval
{: .no_toc }


Music information retrieval (MIR)[[Wiki]](https://en.wikipedia.org/wiki/Music_information_retrieval) 은<br>음악에서 정보를 찾아내고 추출하는 것이 주 목적인 학문 분야이다.
{: .fs-6 .fw-300 }

요즈음에는 신호처리와 기계학습을 주요 툴로 사용하며, 이를 이용해 청각지각과 인지에 관한 여러가지 문제들을 풀고는 한다.
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


# [](#applications)응용 분야

MIR은 다양한 분야의 많은 회사와 연구자들에 의해 개발되었으며, 음악을 분류하고, 음원을 분리하고, 심지어 음악을 제작하는 데도 사용되는 등 여러 응용 분야를 가지고 있다.
{: .fs-5 }

본 페이지에서는 [[MIR 위키피디아]](https://en.wikipedia.org/wiki/Music_information_retrieval)에 따라 응용 분야 다섯가지를 소개하고자 한다.
{: .fs-5 }

## [](#1.1)음악 분류

고전적인 MIR 연구 주제로 가장 대표적인 주제는 음악 분류이다.<br>
음악 분류는 음악들을 분석하여 클래식, 재즈, 록 등 각각의 장르에 따라 분류하는 태스크이다.<br>
비슷한 태스크로, 음악의 느낌에 따른 분위기 분류, 아티스트 분류, 음악 태깅 등이 인기 있는 주제들이다.

## [](#1.2)추천 시스템

멜론, 유튜브 뮤직 등 여러 음원 스트리밍 서비스 사에서 '나만을 위한 음악'을 종종 추천해주고는 한다.<br>
유저가 좋아할만한 음악들을 각 서비스마다의 알고리즘(추천 시스템)을 이용해서 추천해주는 것인데,
이렇듯 음악을 위한 [추천 시스템](https://ko.wikipedia.org/wiki/추천_시스템)들을 주변에서 쉽게 찾아볼 수 있지만, <b>사실 MIR 기술을 기반으로 하는 추천 시스템은 거의 없다.</b><br>

즉, 실제 음악에 대한 정보를 이용해서 추천해주는 시스템은 거의 없다는 말이다.<br>
대신, 유저들의 플레이리스트 데이터를 기반으로 유저들 간의 유사성을 비교하거나, 태그를 이용해 추천을 하곤 한다.<br>

예를 들어 [멜론](https://ko.wikipedia.org/wiki/멜론_(온라인_음악_서비스))의 경우를 살펴보자.<br>
현재 기준으로, 멜론에서는 노래 A를 좋아하는 많은 유저들이 노래 B를 좋아한다면 한 유저가 노래 A를 듣고 좋아요 버튼을 누를 때에 이 유저 또한 노래 B를 좋아할 것이라고 예측하고 노래 B를 추천해주는 추천 시스템을 적용하고 있다.<br>
이는 노래 자체의 정보보다는, 비슷한 음악들을 들은 다른 유저들의 플레이리스트에 영향을 받는 추천 시스템인 것이다.<br>
여담이지만, 사실 적어도 지금까지는 MIR 기술로 음악의 정보를 추출하는 것이 어렵고 비용이 많이 들기에, 멜론에서는 비용도 적게 들고 추천 시스템에 대한 만족도가 훨씬 높은 합리적인 방법을 채택했다고 할 수 있다. [[읽을거리 : 멜론에서 음악 추천을 어떻게 할까? -카카오 추천팀]](https://brunch.co.kr/@kakao-it/342)<br>

비슷한 예로, [판도라](https://ko.wikipedia.org/wiki/판도라_(음악_서비스))는 "여성 가수"나 "강한 베이스라인"과 같이 음악에 특정한 태그를 붙이기 위해 전문가를 이용한다.<br>
그리고 이 태그를 이용해 음악을 추천해주곤 한다.
현재도 많은 추천 시스템들이 멜론과 같이, 청취 기록이 유사한 사용자를 찾고 각각의 플레이리스트에서 유저들이 아직 듣지 않은 음악을 새롭게 추천하곤 한다.<br>

음악 유사도에 대한 MIR 기법은 이제 막 발전해나가고 있는 중이고,<br>
더 나은 추천 시스템을 만들기에 무궁무진한 발전가능성을 가지고 있다.

## [](#1.3)음악 소스 분리와 악기 식별

음악 소스 분리는 혼합된 오디오 신호에서 원래 신호를 분리하는 것이다.<br>
예를 들면, 보컬, 피아노, 드럼 등이 혼합된 오디오 파일에서 피아노 신호만 분리하는 작업을 의미한다.<br>

그리고, 악기 식별은 음악과 관련된 악기를 식별하는 것이다.<br>
말그대로, 어떤 오디오 파일에서의 신호가 피아노 소리인지, 베이스 소리인지, 특정 악기를 식별하는 작업을 의미한다.<br>

이러한 작업들이 발전하면서, 음악을 여러 구성 요소별 트랙으로 분리할 수 있는 MIR 시스템이 다양하게 개발되었다.<br>
이 시스템들을 통해 음악들을 손쉽게 가라오케 트랙으로 만들 수 있게 되었다. 음악에서 보컬을 제거하고 노래방에서 사용할 수 있도록, 그러니까 MR로 사용할 수 있을 정도로 만들 수 있는 것이다.<br>

하지만 아직 완벽하게 해결하지 못한 한계점이 존재하는데,<br>
보컬은 다른 악기들과 주파수 공간이 겹쳐 완벽히 제거하기는 어렵다는 점이다.<br>

## [](#1.4)음악 표기 자동화

음악 표기 자동화는 녹음된 오디오 파일을 [악보](https://ko.wikipedia.org/wiki/악보)나 [MIDI 파일](https://ko.wikipedia.org/wiki/MIDI)과 같은 기호 표기법으로 변환하는 것을 의미한다.<br>
[[기보법(Musical notation)에 대해서 알아보자 -위키피디아]](https://ko.wikipedia.org/wiki/기보법)<br>

이 프로세스에는 여러 가지 오디오 분석 작업이 포함될 수 있는데,<br>
멀티 피치 감지, 시작 감지, 길이 추정, 악기 식별, 화음 정보 추출, 리듬 또는 멜로디 정보의 추출 등이 여기에 사용되는 분석 작업들에 해당된다.<br>

이 작업은 사용하는 악기의 가짓수가 많아질수록, 독립적인 멜로디가 둘 이상의 라인에 동시에 구성되는 [다성음악](https://ko.wikipedia.org/wiki/다성음악)일 수록 어려워진다는 특징이 있다.

## [](#1.5)음악 생성

음악 생성은 MIR를 연구하는 많은 사람들이 가지고 최종적인 목표이다.<br>

지금도 다양한 방법으로 시도되고 있으며, 머신러닝의 발전과 함께 빠르게 발전하고 있는 분야이기도 하다.<br>

이에 관련해서 개인적으로 추천하고 싶은 프로젝트들이 있는데, 아래와 같으니 한번 참고해보면 좋지 않을까 싶다.<br>
* [JukeBox](https://openai.com/blog/jukebox/)<br>
* [MuseNet](https://openai.com/blog/musenet/)<br>

참고로, 두 프로젝트 모두 [Open AI](https://openai.com)라는 인공지능 연구소에서 발표한 프로젝트이다.

---

# [](#methods)주로 사용되는 방법


마찬가지로, [[MIR 위키피디아]](https://en.wikipedia.org/wiki/Music_information_retrieval)에 따라 세가지 방법(Method)들을 소개하고자 한다.

## [](#2.1)데이터 소스

[악보](https://ko.wikipedia.org/wiki/악보)는 음악을 명료하고 논리적으로 설명해주는 수단이지만, 현실적으로 악보를 얻기는 어렵다고 할 수 있다.

MIDI 음악이 소스로 사용되긴하지만, 애초부터 음악을 MIDI 표준을 염두에 두고 만들지 않는 한 MIDI로 변환하는 과정에서 일부 데이터가 손실된다.

오디오 자체를 분석할 때는 WAV, mp3, ogg와 같은 디지털 오디오 포맷을 그대로 사용하곤 한다.

mp3 및 ogg와 같은 디지털 오디오 파일들은 인간의 귀로는 잘 들리지만, 정보가 손실되어 연구에 중요한 데이터가 누락될 수 있다.

그리고, 어떤 인코딩은  자동 분석기가 잘 못 이해할 수 있는 소리를 만들기도 한다.

그럼에도 불구하고 MP3가 어디에나 있다는 것은 이 분야의 많은 연구가 이것들을 원천 자료로 포함한다는 것을 의미했다.

점점 더 웹에서 마이닝된 메타데이터가 MIR에 통합되어 문화적 맥락 내에서 음악에 대한 보다 포괄적인 이해를 돕고 있으며, 최근에는 음악에 대한 소셜 태그 분석으로 구성되어 있습니다.

## [](#2.2)Feature representation

Analysis can often require some summarising, and for music (as with many other forms of data) this is achieved by [feature extraction](https://en.wikipedia.org/wiki/Feature_extraction), especially when the audio content itself is analysed and machine learning is to be applied. The purpose is to reduce the sheer quantity of data down to a manageable set of values so that learning can be performed within a reasonable time-frame. One common feature extracted is the [Mel-Frequency Cepstral Coefficient](https://en.wikipedia.org/wiki/Mel-frequency_cepstral_coefficient) (MFCC) which is a measure of the [timbre](https://en.wikipedia.org/wiki/Timbre) of a piece of music. Other features may be employed to represent the [key](https://en.wikipedia.org/wiki/Tonality#Computational_methods_to_determine_the_key), chords, harmonies, [melody](https://en.wikipedia.org/wiki/Melody), main [pitch](https://en.wikipedia.org/wiki/Pitch_(music)), [beats per minute](https://en.wikipedia.org/wiki/Beats_per_minute) or rhythm in the piece. There are a number of available audio feature extraction tools [Available here](https://www.ntnu.edu/documents/1001201110/1266017954/DAFx-15_submission_43_v2.pdf)

## [](#2.3)Statistics and machine learning
* Computational methods for classification, clustering, and modelling — musical feature extraction for mono- and [polyphonic](https://en.wikipedia.org/wiki/Polyphonic) music, similarity and [pattern matching](https://en.wikipedia.org/wiki/Pattern_matching), retrieval
* Formal methods and databases — applications of automated [music identification](https://en.wikipedia.org/wiki/Music_identification) and recognition, such as [score following](https://en.wikipedia.org/wiki/Score_following), automatic accompaniment, routing and filtering for music and music queries, query languages, standards and other metadata or protocols for music information handling and [retrieval](https://en.wikipedia.org/wiki/Information_retrieval), [multi-agent systems](https://en.wikipedia.org/wiki/Multi-agent_system), distributed search)
* Software for music information retrieval — [Semantic Web](https://en.wikipedia.org/wiki/Semantic_Web) and musical digital objects, intelligent agents, collaborative software, web-based search and semantic retrieval, [query by humming](https://en.wikipedia.org/wiki/Query_by_humming) / [Search by sound](https://en.wikipedia.org/wiki/Search_by_sound), [acoustic fingerprinting](https://en.wikipedia.org/wiki/Acoustic_fingerprinting)
* Music analysis and knowledge representation — automatic summarization, citing, excerpting, downgrading, transformation, formal models of music, digital scores and representations, music indexing and [metadata](https://en.wikipedia.org/wiki/Metadata).