# How the decomposition works

This is a plain description of the current decomposition method. It is not runnable software and not a complete methods section. State as of September 2026.

## The idea

A show file stores what a designer authored, but not in the form a researcher needs. A single cue can change some luminaires and leave others running. An effect can keep moving underneath several cues. A look from the first chorus can come back, slightly changed, in the second. The decomposition turns an authored show into explicit layers over time, so each of these things becomes something one can count, compare and later generate.

## Five steps

1. **Keep the sources and their origin together.** The authored console data, the mapped luminaires and the structure of the audio are kept as versioned inputs. Every derived observation keeps a link back to the source event it came from.
2. **Work out what is active at every moment.** Source events, persistence and the playback context are resolved into an effective state over time. When several cues control the same parameter, the most recent one wins, as on the console. The show explicitly starts from black. Where the actual console output cannot be proven, a known projection is kept and the limitation is recorded.
3. **Separate what holds from what moves.** The state is split into maintained looks, animated layers and short reactions such as accents. A reaction can stay unresolved or supported only by the source. A section that looks complete does not mean that every reaction in it is resolved.
4. **Describe recurrence and development.** A recurring figure keeps its identity across pauses, while each active passage stays separate. The order in which a show develops is recorded, and so are families of related passages within a show. Rare exact repetition is not taken as proof of restraint or of what the designer intended.
5. **Summarise and compare.** Each record gets a fingerprint, and records are compared with each other. The detailed source links and the uncertainty behind every interpretation stay attached.

The current checkpoint contains 101 decompositions and 101 reproduced fingerprints, with 5,050 pairwise comparisons. Reproducing a fingerprint shows that the interpretation is deterministic. It is not a test of the rendered light and not a judgement of artistic quality.

## What the counts mean

The decomposition yields 101 show records, 1,338 sections, 3,164 main cues that change the look, 12,765 accent events and 569 recurrence families within shows.

- The main-cue count leaves out cues that change nothing. It is 5,799 authored main cues minus 2,635 cues that change nothing.
- A main cue that changes the look is not automatically a visually distinct look.
- Accent events are events in the source model, and recurrence families are groupings within one show.
- Some records share the same song. All records of one song stay together when the data is split for evaluation, and cues within a record are not independent observations.

## How the prototype uses the decomposition

The current prototype is a donor transfer. For a new song, it picks one authored show as the donor. It reads the donor's decomposition, fits the donor's structure to the new song's timing and energy, and writes an editable show for the console.

- Only audio from valid, indexed collections counts as audio evidence.
- Reactions that are unresolved or supported only by the source are not used to guide generation.
- Technical checks confirm that the console receives what was declared. Whether the show fits the music is judged separately, in a musical review that is still ongoing.
- Learning composition conventions from all 101 decompositions at once is future work.

## Relation to the proposed layers

The poster proposes ten layers.

1. L1, the context.
2. L2, the dramaturgic arc of the whole song.
3. L3, the visual role of each section.
4. L4, recurrence and variation.
5. L5, the timing of cues and accents.
6. L6, cue content.
7. L7, movement.
8. L8, accents.
9. L9, transitions.
10. L10, a validation step that checks across all of them.

L2 to L9 are proposed content layers, not established independent factors. The layers of the decomposition do not automatically map one to one onto these proposed layers. For every proposed layer, the research has to state what it means, where it comes from, what form it takes and how certain it is.

## Next steps

1. Rebuild authored shows from the smaller layered representation.
2. Generate that representation for unseen songs.
3. Compare the layered model with equally sized flat and collapsed models.
4. Regenerate a selected layer or time region while protected content stays unchanged.

No experimental results for these steps exist yet.

[Poster](../poster/preliminary-poster.pdf) · [Project overview](../README.md) · [wursthorn.org](https://wursthorn.org/) · [Contact](https://wursthorn.org/contact)
