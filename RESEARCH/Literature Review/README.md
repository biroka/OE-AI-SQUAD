Óbudai Egyetem · AI SQUAD **Szakirodalom-kutatási útmutatóLiterature Review Guide**

Kérdések:Questions:\
**Dr. Biró Attila**\
biro.attila@uni-obuda.hu\
vagy Teamsor Teams

Explore · a ciklus első lépéseExplore · the first step of the loop

# Mielőtt építetek, *nézzétek meg, mit tud már a tudomány*.
# Before you build, *find out what science already knows*.

A szakirodalomkutatás (literature review) a témához kapcsolódó publikációk, módszerek, adatszettek, nyílt forráskódok és projektek rendszerezett felkutatása, kritikus értékelése és szintézise. Ebből derül ki a tudomány jelenlegi állása (state of the art), és ebből látszik, hol tud a csapatotok újat hozzátenni.A literature review is the systematic search, critical appraisal and synthesis of publications, methods, datasets, open-source code and projects related to your topic. It establishes the state of the art and shows where your team can add something new.

#### Mit tud már a tudomány?What does science already know?

Elméleti háttér, korábbi eredmények, elfogadott mérési módszerek és metrikák.Theoretical background, prior results, accepted measurement methods and metrics.

#### Milyen modellek, adatszettek, eszközök léteznek?Which models, datasets and tools exist?

Nyílt adatszettek, előtanított modellek, SDK-k, GitHub-repók, benchmarkok.Open datasets, pre-trained models, SDKs, GitHub repos, benchmarks.

#### Mit használhatunk újra, mit javíthatunk?What can we reuse, what can we improve?

A hiányok (research gap) azonosítása, ebből lesz a saját kutatási kérdésetek és a TDK/konferencia-cikk hozzájárulása.Identify the research gap. It becomes your own research question and the contribution of your TDK or conference paper.

### Milyen típusú áttekintést készítsetek?Which type of review should you do?

| TípusType | Mire jóGood for | MódszertanMethod | AI SQUAD-banIn AI SQUAD |
| --- | --- | --- | --- |
| **Narratív áttekintésNarrative review** | Gyors tájékozódás, háttérQuick orientation, background | Szabad, nem reprodukálhatóInformal, not reproducible | Csak az első hétenFirst week only |
| **Strukturált / state-of-the-art áttekintésStructured / state-of-the-art review** | Módszerek, adatszettek, eredmények összevetéseComparing methods, datasets, results | Dokumentált keresés + szűrés + összehasonlító mátrixDocumented search + screening + comparison matrix | Ez az alapelvárásThis is the baseline |
| **Scoping reviewScoping review** | Új, szétszórt terület feltérképezéseMapping a new, scattered field | Arksey & O'Malley (2005) | Pl. okosszemüveg + oktatásE.g. smart glasses + education |
| **Szisztematikus áttekintésSystematic review** | Teljes körű, önálló publikációExhaustive, a publication in its own right | PRISMA 2020, Kitchenham (2007) | Opcionális, ha a cikk maga az áttekintésOptional, if the review is the paper |

**Agilis szemlélet:** a szakirodalom nem egyszeri feladat. Az első 3–4 hétben felépítitek az alapot, utána minden sprintben frissítitek (új preprintek, új repók), és a heti demón röviden beszámoltok róla.**Agile mindset:** the literature is not a one-off task. Build the foundation in the first 3–4 weeks, then update it every sprint (new preprints, new repos) and report briefly at the weekly demo.

Kattintsatok a lépésekreClick through the steps

## A folyamat 7 lépésbenThe process in 7 steps

### Keresőkifejezés-építőSearch string builder

Fogalmanként soroljátok fel a szinonimákat vesszővel elválasztva. Egy fogalmon belül OR, a fogalmak között AND kapcsolat lesz. A `*` csonkolás (pl. `gamif*` = gamification, gamified…). Töltsétek be a saját csapatotok példáját!List synonyms per concept, separated by commas. Synonyms within a concept are joined with OR, concepts with AND. `*` is truncation (e.g. `gamif*` = gamification, gamified…). Load your own team's example!

Példa betöltéseLoad example

1\. fogalomConcept 1

2\. fogalomConcept 2

3\. fogalomConcept 3

Kizárás (NOT)Exclude (NOT)

```

```

Scopusban: TITLE-ABS-KEY( … ) közé téve. Google Scholarban rövidítsétek, mert ott a hosszú lekérdezés pontatlan.In Scopus: wrap in TITLE-ABS-KEY( … ). Shorten it for Google Scholar, which handles long queries poorly.

Nem csak cikkekNot only papers

## Hol keressünk?Where to search

Egy alkalmazott AI-projektnél négyféle forrást kell feltérképezni: tudományos publikációkat, adatszetteket, kódot/modelleket és létező projekteket vagy termékeket. Mindegyikhez más keresőhely tartozik.An applied AI project needs four kinds of sources mapped: scientific publications, datasets, code/models, and existing projects or products. Each has its own search venues.

### Tudományos publikációkScientific publications

[Scopus](https://www.scopus.com)Lektorált folyóiratok és konferenciák; jó szűrők, idézési adatok. Egyetemi hálózatról / könyvtáron keresztül.Peer-reviewed journals and conferences; good filters, citation data. Via university network / library.

[Web of Science](https://www.webofscience.com)Szigorúbban válogatott; a Scopus-szal együtt adja a „hivatalos” lefedettséget.More selective; together with Scopus gives "official" coverage.

[IEEE Xplore](https://ieeexplore.ieee.org) · [ACM Digital Library](https://dl.acm.org)Mérnöki, informatikai, HCI- és jelfeldolgozási konferenciák.Engineering, CS, HCI and signal-processing venues.

[PubMed](https://pubmed.ncbi.nlm.nih.gov)Rehabilitáció, sporttudomány, klinikai validáció. A két rehab-csapatnak kötelező.Rehabilitation, sports science, clinical validation. Mandatory for both rehab teams.

[Google Scholar](https://scholar.google.com) · [Semantic Scholar](https://www.semanticscholar.org)Széles lefedettség, „Cited by” láncolás. Nem lektorált anyagot is mutat, ezért ellenőrizni kell.Broad coverage, "Cited by" chaining. Also lists non-peer-reviewed items, so verify.

[arXiv](https://arxiv.org)A legfrissebb AI-eredmények, de preprint: nincs lektorálva. Nézzétek meg, megjelent-e azóta lektorált helyen.Latest AI results, but preprints: not peer-reviewed. Check whether a peer-reviewed version has appeared since.

### AdatszettekDatasets

[Hugging Face Datasets](https://huggingface.co/datasets)Audio-, kép-, videó- és multimodális adatszettek, adatkártyával (dataset card).Audio, image, video and multimodal datasets, with dataset cards.

[Google Dataset Search](https://datasetsearch.research.google.com)Egyetemi repozitóriumok, Zenodo, PhysioNet stb. egy helyen.University repositories, Zenodo, PhysioNet etc. in one place.

[Zenodo](https://zenodo.org) · [PhysioNet](https://physionet.org) · [Kaggle](https://www.kaggle.com/datasets)Kutatási adatok DOI-val; élettani jelek; versenyadatok (Kaggle-nél a forrás és licenc gyakran bizonytalan).Research data with DOIs; physiological signals; competition data (on Kaggle, provenance and licence are often unclear).

Minden adatszettnél jegyezzétek fel: licenc (kutatási/kereskedelmi), hozzáférés módja (letölthető / EULA / kérvény), alanyok száma, annotáció módja, ismert torzítások.For every dataset record: licence (research/commercial), access route (download / EULA / request), number of subjects, annotation method, known biases.

### Kód és modellekCode and models

[GitHub](https://github.com)Keressetek a cikk címére vagy a módszer nevére. Nézzétek: licenc, utolsó commit, issue-k, reprodukálható-e.Search by paper title or method name. Check: licence, last commit, issues, reproducibility.

[Hugging Face Models](https://huggingface.co/models) · [HF Papers](https://huggingface.co/papers)Előtanított modellek (pl. wav2vec 2.0, ViT), cikkekhez kapcsolt kód és modellek.Pre-trained models (e.g. wav2vec 2.0, ViT), papers linked to code and models.

**SDK-k / SDKs:** Intel RealSense SDK (librealsense), MediaPipe, OpenFace, openSMILE, Meta wearables developer toolkitA gyártói dokumentáció is forrás, de technikai, nem tudományos hivatkozás.Vendor documentation is a source too, but a technical, not scientific, reference.

### Projektek, termékek, kitekintésProjects, products, context

[CORDIS](https://cordis.europa.eu)EU-finanszírozású kutatási projektek (Horizon), eredményekkel és partnerekkel.EU-funded research projects (Horizon), with results and partners.

[Google Patents](https://patents.google.com)Ipari megoldások, főleg okosszemüveg és rehab-eszközök terén.Industrial solutions, especially for smart glasses and rehab devices.

[ClinicalTrials.gov](https://clinicaltrials.gov)Futó klinikai vizsgálatok digitális rehabilitációval.Ongoing clinical trials involving digital rehabilitation.

[MTMT](https://www.mtmt.hu) · OE Könyvtár / LibraryHazai publikációk és szerzők (pl. OE-s kutatók, akiket érdemes megkeresni); a könyvtár segít az előfizetéses adatbázisok elérésében.Hungarian publications and authors (e.g. ÓE researchers worth contacting); the library helps with subscription databases.

### AI-asszisztensek a keresésbenAI assistants in searching

Az Elicit, a Consensus, a Semantic Scholar és az általános chatbotok (ChatGPT, Claude stb.) jók ötletelésre, kulcsszavak bővítésére és absztraktok gyors áttekintésére. Forrásként viszont soha ne idézzétek őket, és egyetlen tőlük kapott hivatkozást se vegyetek át ellenőrzés nélkül: a nyelvi modellek gyakran kitalált (hallucinált) cikkeket, rossz DOI-t vagy rossz évszámot adnak. Minden hivatkozást a kiadó oldalán vagy DOI-n keresztül nyissatok meg. A publikálási helyszín szabályai szerint jelezzétek az AI-eszközök használatát.Elicit, Consensus, Semantic Scholar and general chatbots (ChatGPT, Claude etc.) are useful for brainstorming, expanding keywords and skimming abstracts. Never cite them as a source, and never take a reference from them without checking it: language models often produce invented (hallucinated) papers, wrong DOIs or wrong years. Open every reference on the publisher's site or via its DOI. Disclose AI tool use according to the venue's policy.

Összegyűjteni kevésCollecting is not enough

## Szintézis: a cikkekből tudás leszSynthesis: turning papers into knowledge

A leggyakoribb hiba a „bevásárlólista”: cikkenként egy bekezdés (A ezt csinálta, B azt csinálta). A szintézis ehelyett témák, módszerek és eredmények mentén rendezi az anyagot, összeveti őket, és megmutatja, hol van a hiány.The most common mistake is the "shopping list": one paragraph per paper (A did this, B did that). Synthesis instead organises the material by themes, methods and results, compares them and shows where the gap is.

RosszWeak

„Capecci és mtsai. (2019) létrehozták a KIMORE adatszettet. Vakanski és mtsai. (2018) létrehozták az UI-PRMD adatszettet. Cao és mtsai. kifejlesztették az OpenPose-t.”"Capecci et al. (2019) created the KIMORE dataset. Vakanski et al. (2018) created the UI-PRMD dataset. Cao et al. developed OpenPose."

Felsorol, de nem hasonlít össze, nem értékel, nem mutat hiányt.Lists, but does not compare, evaluate or reveal a gap.

JóStrong

„A nyilvános rehabilitációs adatszettek (pl. KIMORE \[3\], UI-PRMD \[4\]) RGB-D kamerával rögzített mozgásokat és klinikai pontszámokat tartalmaznak, de egyik sem tartalmaz játékos (gamifikált) környezetben végzett gyakorlatokat vagy fáradási címkéket. A mozgásminőség-értékelő módszerek többsége offline működik \[5\], \[6\], így a valós idejű adaptáció még nyitott kérdés.”"Public rehabilitation datasets (e.g. KIMORE \[3\], UI-PRMD \[4\]) contain RGB-D recordings of movements with clinical scores, but none include exercises performed in a gamified setting or fatigue labels. Most movement-quality assessment methods run offline \[5\], \[6\], so real-time adaptation remains an open question."

Csoportosít, összevet, és megfogalmazza a hiányt, ami a saját hozzájárulásotokat indokolja.Groups, compares and states the gap that justifies your contribution.

### Az eszköz: az összehasonlító (koncepció-) mátrixThe tool: the comparison (concept) matrix

Egy közös táblázat (Google Sheets vagy a GitHub-repóban egy CSV), ahol minden sor egy forrás, minden oszlop egy összehasonlítási szempont. Ebből születik a cikk „Related Work” táblázata. Példa (rövidítve, a rehab-csapatok témájából):A shared table (Google Sheets or a CSV in the GitHub repo) where each row is a source and each column a comparison criterion. It becomes the "Related Work" table of your paper. Example (abridged, from the rehab teams' topic):

| ForrásSource | SzenzorSensor | Adat (n)Data (n) | MódszerMethod | MetrikaMetric | Valós idő?Real-time? | Gamifikáció?Gamified? | KorlátLimitation |
| --- | --- | --- | --- | --- | --- | --- | --- |
| KIMORE \[Capecci 2019\] | Kinect v2 (RGB-D) | 78 alany78 subjects | Adatszett + klinikai pontszámDataset + clinical score | Klinikai skálaClinical scale | – | ✕ | 5 gyakorlat, alsó hát5 exercises, low back |
| UI-PRMD \[Vakanski 2018\] | Vicon + Kinect | 10 alany10 subjects | Adatszett, helyes/hibás ism.Dataset, correct/incorrect reps | – | – | ✕ | Egészséges alanyokHealthy subjects |
| BlazePose \[Bazarevsky 2020\] | RGB | – | 33 pontos pózbecslés33-keypoint pose | PCK | ✓ (mobil) | ✕ | Mélység becsültDepth estimated |
| Saját munkaOur work | RealSense + IMU | ? | ? | ? | ✓ | ✓ | ? |

A számadatokat mindig az eredeti cikkből ellenőrizzétek, mielőtt a saját anyagotokba kerülnek.Always check figures against the original paper before they go into your own work.

#### 1. Tematikus csoportosítás1. Group by theme

Pl. „szenzorok és adatgyűjtés”, „mozgásminőség-értékelés”, „adaptáció és motiváció”. Ezek lesznek a Related Work alfejezetei.E.g. "sensors and data collection", "movement-quality assessment", "adaptation and motivation". These become your Related Work subsections.

#### 2. Összevetés és értékelés2. Compare and evaluate

Mely módszer mely metrikán jobb, milyen adaton? Összevethetők-e az eredmények (azonos adatszett, protokoll)? Mi a minta mérete, a validáció módja?Which method wins on which metric, on what data? Are results comparable (same dataset, protocol)? What is the sample size and validation scheme?

#### 3. Hiány (gap) és hozzájárulás3. Gap and contribution

Mondjátok ki: „A szakirodalomban nem találtunk olyan munkát, amely X-et Y körülmények között Z-vel mér.” Ebből jön a kutatási kérdés és a hipotézis.State it: "We found no work that measures X under Y conditions with Z." This yields the research question and hypothesis.

**Hasznos mondatpanelek:** „A legtöbb korábbi munka … ezzel szemben …”, „Az eredmények ellentmondásosak: … \[3\] szerint …, míg \[5\] …”, „Ezek a megközelítések nem veszik figyelembe …”, „Tudomásunk szerint ez az első munka, amely …” (ezt csak alapos keresés után írjátok le!).**Useful sentence frames:** "Most prior work … in contrast …", "Findings are mixed: \[3\] reports …, whereas \[5\] …", "These approaches do not account for …", "To the best of our knowledge, this is the first work that …" (write this only after a thorough search!).

Mire figyeljetek az anyaggyűjtésben?What to watch for when collecting

## Csapdák, minőség, etikaPitfalls, quality, ethics

Kitalált vagy hibás hivatkozások (AI-hallucináció)Invented or wrong references (AI hallucination)kritikuscritical

Ha egy hivatkozás nem nyitható meg DOI-n vagy a kiadó oldalán, nem létezik. Egy nem létező hivatkozás a TDK-dolgozatban vagy konferenciacikkben komoly tudományos integritási probléma.If a reference cannot be opened via its DOI or publisher page, it does not exist. A non-existent reference in a TDK paper or conference submission is a serious research-integrity problem.

Másodkézből idézésSecond-hand citingkritikuscritical

Csak olyat idézzetek, amit legalább az absztrakt, a módszertan és az eredmények szintjén ti magatok elolvastatok. Ha egy állítás egy review-ból származik, az eredeti forrást keressétek meg.Cite only what you have read yourselves, at least the abstract, method and results. If a claim comes from a review, track down the original source.

Ragadozó (predatory) folyóiratok és konferenciákPredatory journals and conferenceskritikuscritical

Jelek: gyors „lektorálás”, kéretlen e-mailes felkérés, homályos szerkesztőbizottság, Scopus/WoS-ban nem szerepel. Ellenőrzés: Scopus Sources lista, DOAJ, a kiadó és a konferencia (IEEE, ACM, Springer, Elsevier, MDPI esetén a konkrét folyóirat) hírneve, illetve kérdezzétek a mentort.Signs: very fast "review", unsolicited email invitations, vague editorial board, not indexed in Scopus/WoS. Check: Scopus Sources list, DOAJ, the publisher's and venue's reputation (for MDPI, the specific journal), or ask your mentor.

Preprintek és visszavont cikkekPreprints and retracted papersfontosimportant

Az arXiv-cikkeknél nézzétek meg, van-e lektorált változat, és azt idézzétek. Visszavonásokat a kiadó oldalán vagy a Retraction Watch adatbázisban ellenőrizhettek (a Zotero is figyelmeztet).For arXiv papers, check for a peer-reviewed version and cite that. Check retractions on the publisher's page or the Retraction Watch database (Zotero also warns you).

Nem összevethető eredményekNon-comparable resultsfontosimportant

95% pontosság az egyik adatszeten nem jobb, mint 70% egy másikon. Figyeljétek: azonos adatszett és felosztás? Alany-független (subject-independent) validáció? Kiegyensúlyozatlan osztályok mellett accuracy helyett F1 / UAR. Egy alany adatai ne kerüljenek egyszerre a tanító és a teszt halmazba (data leakage).95% accuracy on one dataset is not better than 70% on another. Check: same dataset and split? Subject-independent validation? With imbalanced classes use F1 / UAR instead of accuracy. Data from one subject must not appear in both training and test sets (data leakage).

Adatlicenc és adatvédelem (GDPR)Data licences and privacy (GDPR)fontosimportant

Az arc, a hang, a mozgásminta és az egészségügyi adat személyes, sokszor különleges kategóriájú (biometrikus, egészségügyi) adat. Saját adatgyűjtéshez tájékoztatás, írásos beleegyezés és szükség esetén etikai engedély kell, amit a mentorral kell egyeztetni. Kutatási licencű adatszetten tanított modell nem használható kereskedelmi célra.Faces, voices, movement patterns and health data are personal, often special-category (biometric, health) data. Your own data collection needs participant information, written consent and, where required, ethics approval: agree this with your mentor. A model trained on a research-only dataset cannot be used commercially.

EU AI Act: érzelemfelismerés oktatásban és munkahelyenEU AI Act: emotion recognition in education and the workplacefontosimportant

Az EU AI Act (2024/1689 rendelet) 5. cikke tiltja az érzelemfelismerő rendszerek alkalmazását munkahelyen és oktatási intézményben (orvosi és biztonsági kivételekkel). Ez a 14-es és a 8-as csapatot közvetlenül érinti: kutatási prototípus készülhet, de a cikkben tárgyaljátok a jogi és etikai kereteket, és ne tervezzetek diákok érzelmeit monitorozó oktatási alkalmazást.Article 5 of the EU AI Act (Regulation 2024/1689) prohibits emotion-recognition systems in workplaces and educational institutions (with medical and safety exceptions). This directly affects Teams 14 and 8: a research prototype is fine, but discuss the legal and ethical framing in your paper and do not design an educational application that monitors students' emotions.

Megerősítési torzítás és „cherry picking”Confirmation bias and cherry-pickingfontosimportant

Az ellentmondó és negatív eredményeket is gyűjtsétek. A kizárás okát mindig rögzítsétek (pl. „nem RGB-D”, „nem emberi alany”), így a szűrés átlátható és megismételhető.Collect contradicting and negative results too. Always record the reason for exclusion (e.g. "not RGB-D", "no human subjects") so screening is transparent and repeatable.

Plágium és saját szövegPlagiarism and your own wordsfontosimportant

Ábrát, táblázatot vagy szó szerinti mondatot csak jelölve és hivatkozva vegyetek át. Jegyzeteléskor különítsétek el a szó szerinti idézetet (idézőjel + oldalszám) a saját összefoglalótoktól, így később nem keveredik.Reuse figures, tables or verbatim sentences only when marked and cited. When taking notes, separate verbatim quotes (quotation marks + page) from your own summaries so they don't get mixed up later.

### Gyors forrásértékelés (5 kérdés)Quick source appraisal (5 questions)

1. Hol jelent meg? Lektorált, indexelt (Scopus/WoS) helyen?Where was it published? Peer-reviewed, indexed (Scopus/WoS)?
2. Mekkora és milyen a minta (alanyok száma, demográfia, egészséges vagy páciens)?How large and what kind of sample (number of subjects, demographics, healthy or patients)?
3. Mi a referencia (ground truth), és ki annotált?What is the ground truth, and who annotated it?
4. Elérhető-e a kód és az adat, reprodukálható-e?Are code and data available, is it reproducible?
5. Milyen korlátokat ír a szerző, és ti milyet láttok még?Which limitations do the authors state, and which others do you see?

Publikálásra készenReady for publication

## Pontos hivatkozásAccurate referencing

A hivatkozásokat az első naptól hivatkozáskezelőben gyűjtsétek. A cikk írásakor már csak be kell illeszteni őket. Mérnöki konferenciákon és a legtöbb TDK-szekcióban az IEEE stílus az alapértelmezett, de mindig a felhívás (call for papers) sablonja dönt.Collect references in a reference manager from day one. When writing, you only need to insert them. IEEE style is the default for engineering conferences and most TDK sections, but the call for papers template always decides.

#### Zotero + Better BibTeX

Csapatonként egy közös **Zotero Group Library**. A böngészőbővítménnyel egy kattintással mentitek a cikket a metaadatokkal együtt. A Better BibTeX automatikusan frissülő `.bib` fájlt exportál.One shared **Zotero Group Library** per team. The browser connector saves a paper with its metadata in one click. Better BibTeX exports an auto-updating `.bib` file.

#### Overleaf + BibTeX

A `references.bib` az Overleaf-projektben van, a szövegben `\cite{capecci2019kimore}`. A hivatkozáslistát a LaTeX generálja, így nem lehet elírni a sorszámokat.`references.bib` lives in the Overleaf project, and the text uses `\cite{capecci2019kimore}`. LaTeX generates the reference list, so numbering can't go wrong.

#### Egységes kulcsok és címkékConsistent keys and tags

Kulcs: `szerzőÉvSzó` (pl. `gong2022vocalsound`). Címkék a Zoteróban: `dataset`, `method`, `review`, `included`, `excluded`. Így a szűrés is a Zoteróban követhető.Key: `authorYearWord` (e.g. `gong2022vocalsound`). Zotero tags: `dataset`, `method`, `review`, `included`, `excluded`, so screening is tracked in Zotero too.

### Egy IEEE-hivatkozás felépítéseAnatomy of an IEEE reference

\[3\] M. Capecci *et al.*, “The KIMORE dataset: KInematic assessment of MOvement and clinical scores for remote monitoring of physical REhabilitation,” *IEEE Trans. Neural Syst. Rehabil. Eng.*, vol. 27, no. 7, pp. 1436–1448, Jul. 2019, doi: 10.1109/TNSRE.2019.2923060.

Szerzők (3 felett: et al.)Authors (more than 3: et al.)Cím idézőjelbenTitle in quotesFolyóirat/konferencia dőlten, rövidítveJournal/conference in italics, abbreviatedKötet, szám, oldalakVolume, issue, pagesDátumDateDOI

A DOI-t a doi.org-on nyissátok meg, és vessétek össze a metaadatokat. Ez az egyetlen biztos ellenőrzés.Open the DOI on doi.org and compare the metadata. This is the only reliable check.

### Nem csak cikket kell hivatkozniIt's not only papers you cite

**Adatszett és szoftver:** mindig az adatszett/eszköz *eredeti cikkét* idézzétek (ha van), és ha a licenc előírja, a megadott hivatkozást is. Szoftvernél adjátok meg a verziót vagy commitot, weboldalnál a letöltés dátumát. A saját kódotokat a GitHub-repóban egy `CITATION.cff` fájllal tehetitek idézhetővé, Zenodón DOI-t is kaphat.**Datasets and software:** always cite the dataset/tool's *original paper* (if any), plus the citation required by its licence. Give the version or commit for software, the access date for web pages. Make your own code citable with a `CITATION.cff` file in the GitHub repo; Zenodo can mint a DOI for it.

Kiindulópontok, nem kész listaStarting points, not a finished list

## Csapatonkénti példákExamples per team

Válasszátok ki a csapatotokat. Minden példahivatkozás ismert, sokat idézett munka, de a lista szándékosan hiányos: a ti feladatotok bővíteni, és mindegyiket ellenőrizni (DOI, év, oldalszám).Pick your team. Every example reference is a well-known, widely cited work, but the list is deliberately incomplete: your job is to extend it and verify each one (DOI, year, pages).

A heti ritmushoz igazítvaAligned with the weekly rhythm

## Ütemterv és ellenőrzőlistaTimeline & checklist

W1

#### FelderítésScoping

Kutatási kérdés, fogalmak, 5–10 kulcscikk, keresőkifejezések. Zotero-csoport és mátrix létrehozása.Research question, concepts, 5–10 key papers, search strings. Set up Zotero group and matrix.

W2

#### Keresés és szűrésSearch & screen

Keresés 3+ adatbázisban, cím/absztrakt-szűrés, hólabda, adatszett- és repó-keresés.Search 3+ databases, title/abstract screening, snowballing, dataset and repo search.

W3

#### KivonatolásExtraction

Teljes szöveg olvasása, mátrix kitöltése, adatszettek licencének ellenőrzése, baseline kiválasztása.Full-text reading, fill the matrix, check dataset licences, choose a baseline.

W4

#### SzintézisSynthesis

Related Work vázlat Overleafben, gap megfogalmazása, bemutatás a heti demón. Utána sprintenként frissítés.Related Work draft in Overleaf, state the gap, present at the weekly demo. Then update every sprint.

### Kész vagyunk?Are we done?

A pipák csak a saját böngészőtökben tárolódnak.Ticks are stored only in your own browser.

KérdésekQuestions

**Dr. Biró Attila** · biro.attila@uni-obuda.hu · vagy Microsoft Teamsor Microsoft Teams
