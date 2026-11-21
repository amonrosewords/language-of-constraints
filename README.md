*Specific constraint prompting: how to direct generative AI*

# The Language of Constraints

A manual for directing generative systems without surrendering authorship: the grammar, music in practice, and images.

A. Monrose, with Claude · November 2026

> **A generative system given freedom will give you the average.**
>
> **Not because it lacks capability. Because the average is what freedom selects for.**
>
> **Everything that follows is a grammar for taking freedom away.**

> I call this **specific constraint prompting**. The method videos show it one song at a time: a beginner prompt beside a precise one, the same lyric, the same model. Thirteen episodes are finished; the series runs on YouTube every Thursday from November 19, 2026.

This is a manual about directing machines that generate — music, prose, images, code, analysis. It contains no prompts to copy. Copied prompts stop working when the tool updates, and they teach nothing. What it contains is a grammar: a set of instruction types that behave predictably across systems, and a method for finding out which ones a particular system respects.

It grew out of a specific project — twenty-four songs, written as lyrics across twenty-five years and given music in one — and the failures were logged as carefully as the successes. Where a principle came from a failure, that's said.

I call the practice **specific constraint prompting**: direct the machine by naming what must be true and what must never happen, rather than describing a mood.

The claim is not that this makes a machine creative. It is that a person with a clear vision, a large amount of specific knowledge, and the discipline to remove options can direct a fluent, tasteless, tireless instrument toward something neither of them would have produced alone. **The machine supplies fluency. You supply the reason anything should exist at all.**

**How this manual is laid out.** Part One is the grammar: thirteen principles that hold for any generative tool. Part Two is the grammar at work on songs, with the prompt template, two case studies, and what a new model version changed. Part Three tests the grammar on pictures. Music readers can start with Part Two and follow its pointers back; the principles are stated once, in Part One.

## Part One · The grammar

### Why freedom yields the average

These systems work by predicting what is likely. Given a broad instruction, an enormous number of outputs satisfy it, and the system selects from the densest region of that space — which is, by definition, the most typical answer. Vagueness is not an invitation to invent. It is an instruction to interpolate.

This is why asking for originality fails so reliably. *Unique*, *original*, *unconventional* and *surprising* are not instructions. They are compliments. They describe how you would like to feel about the result, and they tell the system nothing about what to do.

> **Asks for originality:** Make it unique and unconventional.
>
> **Removes the conventional:** The chorus appears once, at the end. No instrument enters after the first minute. End before the phrase resolves.

The second contains no word meaning "original." It is original because the ordinary answers have been made unavailable.

> **Creativity is not what you add to a prompt. It is what remains after you have closed the obvious routes.**

#### The test that shows it

This is worth running yourself, because the result is more convincing than any argument.

Take a short piece of fiction and ask a language model to write what happens next — six times, changing only one word each time. *Chronicle it. Weave it. Draft it. Craft it. Write it. Continue it.*

The six outputs differ visibly. One is dry and formal, another loose, a third reaches for lyricism. Verb choice plainly affects the surface, and anyone who says word choice doesn't matter is wrong.

Then read beneath the surface. In the run this manual is drawn from, all six opened the same way, moved through the same middle, and arrived at the same ending — the ending the material was already pulling toward. Scored blind on nine dimensions, they ranged from competent to clichéd, and the weakest delivered every beat the story's gravity demanded: the trembling voice, the tears, the stated forgiveness.

> **Six verbs. One skeleton.**

A seventh version used the plainest verb of all — *write* — and added five structural instructions: begin on the second day rather than the first; never allow the two characters to be alone in a room; do not resolve the central contradiction; ban the confession scene; end on a physical object rather than a stated feeling.

It shared none of the others' architecture. It began where they never would have begun, kept the estranged pair on opposite sides of a doorway for the entire piece, held two irreconcilable truths without dissolving either, and ended on a screen door swinging inward, pausing, and settling back against its frame — doing by image what the six had done by statement.

The six differed in coat. The seventh had different bones.

> **A better verb changes what a work wears. A constraint changes its skeleton — and cliché lives in the skeleton.**

### 01 · Architecture before adjectives

Specify the shape of the thing, not the feeling it should produce.

Cliché enters through form far more than through texture. A song defaults to verse–chorus–verse–chorus–bridge–chorus. An essay defaults to introduction, three supporting points, conclusion. An image defaults to a centred subject at eye level. Change the texture and you get a familiar shape in new clothes. Change the shape and everything downstream must be reinvented.

Architecture is also the most reliably obeyed instruction type. Delivery notes, mood words and fine performance detail are frequently ignored or only partly honoured. Structural rules — what goes where, what appears once, what never returns — survive generation after generation.

> **Spend your precision where it is obeyed.**

#### What an architectural constraint looks like

- The thing that would normally arrive first arrives last.
- The element that would normally repeat appears exactly once.
- Nothing is added after a certain point; only removed.
- It ends mid-gesture, without resolving.

### 02 · Contradiction

Give two instructions that pull against each other, and one rule for how they resolve.

When every descriptor points the same way — warm, intimate, acoustic, organic — the system retrieves a single coherent cluster it has seen many times. When two descriptors are incompatible, there is no cluster. It has to construct something.

    familiar element A
    + incompatible element B
    + one rule for how they meet

A lullaby's volume carrying violent content. A children's melody at funeral pace. A formal legal register describing something trivial. A photograph's realism applied to an impossible object. The tension must be productive rather than arbitrary — ask which element should feel human and which mechanical, and where the audience should feel the instability.

The most useful contradictions come from the content itself. If the material already contains a tension, name it and let the form carry it. Imposed strangeness announces itself; discovered strangeness feels inevitable.

### 03 · Narrow reference

Name a specific situation, not a category.

Categories are too large to constrain anything. "Ambient," "noir," "corporate," "minimalist" each contain thousands of typical answers. A narrow reference points at a small neighbourhood, and the best ones specify several dimensions at once: period, place, physical circumstance, equipment, limitation, and the state of the person making it.

> **Category:** A moody indie sound.
>
> **Situation:** A one-microphone room recording with audible chair movement, made by musicians who are still unsure of the arrangement.

Note what the second supplies that the first cannot: a reason for the imperfections. Constraints that carry a *cause* generate consistent detail, because the system can reason from the situation to its consequences.

### 04 · Negative space

Name the defaults you know are coming, and forbid them.

Every system has habits — things it adds unrequested because they are statistically safe. Reverb. Rising strings. Symmetrical composition. A summarising final paragraph. A list of three. An upbeat conclusion. You learn them by generating a few times and noticing what keeps appearing.

A prohibition is often worth more than a description, because it is unambiguous. "Make it restrained" is interpretable. "No element may enter after the first third" is not.

Three cautions. Do not ban everything — excessive prohibition produces thin, lifeless output rather than disciplined output. And place negatives late, after the positive description, where they read as fences rather than as the subject. Finally, ban things, not qualities: an instrument, an object or a section can be cleanly absent, but forbidding a manner (*no emotion*, *never spoken*) names it, and naming it invites it.

### 05 · Relational instruction

Describe how each part differs from the one before, rather than scheduling events.

This is the least obvious principle here and among the most useful. Systems handle *comparison* far more reliably than they handle *timing*.

> **Scheduled:** Add tape flutter at 1:40. Increase reverb in the third section.
>
> **Relational:** Each section is hazier than the one before it, edges softening, until the last is fully blurred.

The scheduled version requires the system to track absolute position, which it does badly. The relational version gives it a direction of travel, which it follows well — and even a partial success preserves the arc, because the contrast between beginning and end gives it a target to aim at.

This generalises. *Each paragraph plainer than the last.* *Each frame emptier than the one before.* *Every function simpler than the one it replaces.* Trajectory is more robust than schedule.

### 06 · Format is instruction

How the input is laid out changes the output, whether or not you intend it.

Line breaks become phrase boundaries. A line alone becomes emphasis. Crowded syllables become rushed delivery. An incomplete sentence becomes a suspension. In text generation, a heading changes register; a numbered list produces enumerated thinking; an example shapes everything after it more powerfully than any adjective.

    I thought I heard you say
    no
    not yet

That white space is an instruction. It was never typed as one.

The practical consequence: proofread your input for accidental instructions. A stray list will produce a list. An example chosen carelessly will be imitated in every respect, including the ones you didn't notice.

### 07 · Semantic gravity

Every word drags its neighbourhood in with it.

Words do not carry only their meanings. They carry the company they keep in the training data. A nylon-string guitar plus a waltz plus a ballroom produced Mediterranean romance in a song where no country was ever named — because those three terms sit close together in a region the system knows well.

Bagpipes carry Scotland. "Cathedral" carries Europe. "Startup" carries a visual style, a vocabulary and a set of assumptions. "Journey" carries a whole narrative arc. None of this is a malfunction; it is what association does.

Two forms of gravity are easy to miss. **Parts add up to a whole you never named:** a pedal steel guitar, a slow waltz and a baritone guitar produced a country ballad without the word "country" appearing anywhere. Describing components instead of a genre only helps if the components don't belong to that genre. **Images carry timing:** "a heartbeat felt through a mattress" produced sleeping-speed music, and "funeral pace" pulled a song somewhere strange. A number, such as "6/8 at about 60 beats per minute," carries no picture to interpret.

Words also carry people. "Chanted" brought a crowd into a song meant for one voice; "a small gathering of friends" put a group in the room for every verse. Before generating, ask who each word invites in.

#### How to work with it

- Before generating, read your own instruction and ask what each term smuggles in.
- If a drift is unwanted, anchor the idiom rather than replacing the element: name *how* the thing should be done, once, and only swap the element if that fails.
- If the drift is interesting, keep it. A recurring unwanted association is a free reference point you hadn't thought of.

### 08 · Elements persist

Anything introduced tends to stay. Schedule presence by explicit rule, not by narrative.

A second voice, once added, tends to remain for the whole piece. A visual element, once present, recurs. A concept introduced in paragraph one colours paragraph nine. These systems maintain what they establish.

So instructions phrased as story — *after she leaves, the second voice disappears* — fail, because the system is not tracking a plot. Instructions phrased as binary rules — *the second voice appears only in the first refrain and the final two lines, and nowhere else* — work far better.

And when it still fails, the fallback is to remove the element entirely and let its absence carry the meaning. A song about someone gone is often better without her voice in it at all.

A newer model made the fallback the rule. On it, even a careful binary rule could not keep a group of backing voices to the choruses: mentioned anywhere, they sang everywhere. Removing them entirely kept the singer alone, and the song was more intimate for it. When the rule fails, removal is not a compromise; test it first. If the element really must come and go, control it after generation, from separated stems, rather than in the instruction.

### 09 · One variable at a time

Change everything and you learn nothing.

This is the single most common failure, and it looks like diligence. A result disappoints, so the whole instruction gets rewritten — new structure, new reference, new constraints. The next result differs, and it is impossible to say why. Nothing is learned, and nothing that worked can be reproduced.

The discipline is straightforward and unglamorous. Keep every instruction that worked. Change exactly one. Generate. Record what happened.

| Version | Changed            | Result                    | Verdict |
|---------|--------------------|---------------------------|---------|
| A       | No opening section | Strong start, weak middle | Keep    |
| B       | Removed reverb     | More intimate             | Keep    |
| C       | Single chorus      | Ending felt abrupt        | Modify  |

The log is not bureaucracy. It is the only way the work becomes cumulative rather than repetitive — and it is what converts a tool you are guessing at into an instrument you know.

### 10 · Read divergence before correcting it

When the output differs from the instruction, check the source material before assuming the machine was wrong.

A vocal came back resigned where the instruction specified tense. That looked like a failure. It wasn't: the lyric names exhaustion as the mechanism of captivity, and rage would have implied enough energy to leave. The system had read the content more accurately than the instruction had.

This happens often enough to be worth a habit. A divergence is evidence about one of three things — a flaw in the instruction, a limit of the system, or something true in the material that you had not consciously registered. The third is the valuable case and the easiest to overwrite.

> **Before you correct the machine, check whether it has understood your material better than your instruction did.**

### 11 · Curate the outlier

Constraints change probabilities. They do not produce results. Generate many; keep the one with a genuine surprise in it.

The working sequence: generate several versions, discard the polished and expected ones, find the version containing one decision you did not anticipate, preserve that decision, and rebuild around it.

The strangest result is not automatically the best. You are looking for productive unfamiliarity, not disorder. The tests:

- Does the unusual choice reveal something about the material?
- Does it create tension that can be sustained?
- Does it survive repeated exposure?
- Does it feel intentional, even though it wasn't?
- Or is it merely broken?

One instance is worth recording. An instruction specified a voice that never rises, not even at the refrains. On one take it rose — for a single line near the end, a brief flash of anger, and then fell back into resignation. The instruction had been violated. The result was better. It was kept.

No prompt produces that. A person hears it and decides.

### 12 · Borrow a mechanism from something you know cold

Don't ask for surprise. Hand over a procedure for producing it, taken from a domain you understand in your bones.

Asking a system to be surprising produces noise, because surprise is a property of a result rather than an action. But surprise has *shapes*, and a shape can be specified — by naming a mechanism the system already understands from somewhere else.

> **Asks for a property:** Take surprising turns.
>
> **Supplies a mechanism:** The melodic motifs should take surprising turns like play-on-words phrases.

A pun is a well-understood move: a phrase pivots on a hinge, meaning one thing and then snapping to another. Saying *turn like a pun* transfers that procedure from language into music. The result is controlled freshness rather than randomness, because the analogy constrains the swerve to a *kind* of swerve.

The important part is where the analogy comes from. That one worked because puns are native to a writer — wordplay is a domain he knows without thinking. A magician would reach for misdirection; a comedian for timing; a carpenter for a joint that hides its own fastening. **The mechanism has to be drawn from a competence you actually possess**, because you need to know how it behaves, not merely what it's called. Borrowed from outside, the analogy lands vague and does nothing.

This is the clearest case of the tool amplifying what you already are. Your depth in an unrelated field becomes a source of instructions nobody else would write.

### 13 · Describe the observable, not the role

Say what the result should do, in terms anyone can check. Don't hand the system a character to play.

A role invites a performance. "A witness telling what he saw" sounds precise, but a witness has feelings about what he witnessed, and the system sang them. "Controlled anger, biting off the ends of lines" is a set of acting techniques, and a literal system executes techniques one by one: mannerisms with no person underneath. What worked was behaviour you can verify by listening: *singing on a narrow, level melody, exactly the same tone from first line to last, no emphasis.*

> **A role to play:** Write as a sceptical expert.
>
> **Behaviour to check:** Every claim carries a number or a source. No hedging words. State the strongest objection before the conclusion.

#### Three habits that go with it

- **Describe the target, not the thing to avoid.** A strong instruction can overshoot, and the reflex is to ban the overshoot. For a quality or a manner, that backfires: *never spoken or half-spoken* produced half-singing, and *no emotion* produced a lifeless voice. Name what you want instead, as something observable: *a narrow, level melody.* Push prose toward plain and it turns curt; ask for *short sentences that still connect*, not for *no long sentences*.
- **Point; don't ask the system to detect.** "Whenever the story returns to the real world" asks it to interpret meaning, and it guesses. "The third verse, the fourth verse and the outro" asks it to count, which it does well.
- **Check your instructions against each other.** An early, broad rule beats a later exception. Something described as never stopping will not stop dead later, however clearly the stop is requested. Read the whole instruction for conflicts before generating.

> **A role is something to perform. A behaviour is something to check.**

### How many constraints

Specificity has an optimum, and it is lower than enthusiasm suggests. The counts below are a working rule of thumb from one project, not a measurement. A constraint means one decision about the work, however many clauses it takes to state: count decisions, not commas.

| Count | Behaviour                                                                |
|-------|--------------------------------------------------------------------------|
| 1–2   | Too much freedom. You get the average.                                   |
| 3–5   | The range where instructions are reliably honoured.                      |
| 6–9   | Partial compliance. Some instructions silently dropped.                  |
| 10+   | The system begins selecting which to obey. Diagnosis becomes impossible. |

Past the threshold you lose more than compliance — you lose the ability to know which instruction produced which effect, which ends the possibility of learning anything. If you have more ideas than will fit, distribute them across separate generations and compare. That is not a compromise. It is the experiment.

### When the model updates

Re-test old instructions. A more literal model punishes the looseness a looser one forgave.

When a new version of a tool arrives, the first reaction is often that it is worse. Sometimes it is. But a model that follows instructions more closely will expose every vague phrase that the previous one quietly rescued with instinct. In the project behind this manual, six songs that had sounded like near misses were re-made on a newer model. Each one improved once its prompt was read again, line by line, for what it literally said. One take that had been approved months earlier turned out, to a more practised ear, to have been a near miss all along.

So treat an update as a reason to re-read, not to re-write. Run the old instruction, listen for exactly where it drifts, and fix that one place. Judge on at least two generations, because the same instruction can miss once and land the next time. And check what you actually submitted: one fix in this project was credited to a clause that had never made it into the prompt.

### Manner and architecture

Constraints operate at two levels, and confusing them is why good prompts stop improving.

A **manner constraint** is global. It sets how the system moves through any material — interleave rather than blur, restrain rather than swell, plain rather than ornate. It is reusable, portable between works, and it raises the floor of everything you make.

An **architectural constraint** is local. It is derived from one specific work — from that piece's own content and the particular cliché that piece is about to fall into. It cannot be carried to the next work, because the next work has different gravity. It raises the ceiling of one thing.

|          | Manner            | Architecture       |
|----------|-------------------|--------------------|
| Scope    | Any work          | This work          |
| Reusable | Yes               | No, by design      |
| Source   | Accumulated taste | Reading this piece |
| Effect   | Raises the floor  | Raises the ceiling |

Originality is a local property, because surprise is measured against an expectation, and expectations are set by content. An arrangement that shrinks at the chorus is startling in a devotion song precisely because devotion songs build. A global instruction cannot aim that, because it does not know what the material leads a listener to expect. It can inject undirected freshness; it cannot break *this* cliché.

Contradiction is unavailable at the global altitude for the same reason: it needs one half of the collision to come from the content. You can say *be surprising*. You cannot say *a lullaby delivered with menace* unless you know there is a lullaby.

> **A manner constraint is an answer, and it is the same for every piece. An architectural constraint is a question, asked again each time.**

The complete instrument stacks four layers: a manner instruction, one well-chosen pointing word, an architecture derived from the specific work, and two or three targeted prohibitions. Most people hold one or two of these and wonder why the results plateau.

### Prose, code and analysis

The grammar does not belong to any one medium. What changes is the vocabulary of each constraint type.

#### Prose

**Architecture:** the conclusion appears first; no paragraph exceeds three sentences; the argument is never stated, only demonstrated. **Contradiction:** a bureaucratic register describing something tender. **Narrow reference:** not "formal," but "a field report written by someone who expects to be overruled." **Negatives:** no summarising final paragraph, no list of three, no rhetorical questions.

Images get their own part: see Part Three.

#### Code

**Architecture:** no function longer than fifteen lines; no shared state; errors handled at the boundary only. **Negatives:** no new dependencies; no abstraction introduced for a single use. **One variable at a time** is not a suggestion here — it is how debugging works, and it is the same principle.

#### Analysis and thinking

**Architecture:** state the strongest counter-argument before the conclusion. **Contradiction:** argue the case you find least congenial, at full strength. **Negatives:** no hedging, no both-sides framing, no appeal to consensus. **Curate the outlier:** generate several framings and keep the one that makes you uncomfortable, because that is the one carrying information you didn't already hold.

## Part Two · Music in practice

AI music systems produce familiar results because familiar results are statistically safe. Ask for an “emotional cinematic pop ballad” and the system needs to invent almost nothing. It retrieves a large cluster of common choices: a short intro, verse–chorus structure, rising strings, layered vocals, a final key change, a polished reverberant mix.

The solution is not more unusual adjectives or more forceful verbs. The reliable way to move a system away from cliché is to **reduce the number of acceptable outcomes**.

The goal is not to control every musical detail. It is to define a small set of strong boundaries within which the system must make less predictable decisions.

### 2.1 · The limits of verb choice

Verbs help, especially when they describe physical or musical processes:

- fracture
- stagger
- withhold
- interrupt
- suspend
- smear
- circle
- collapse
- whisper
- resist
- lurch
- unravel

> **Describes an effect:** Create an emotional vocal.
>
> **Describes behaviour:** Let the vocal enter late, interrupt its own phrases, and withhold the final word of each couplet.

But verb choice is not the primary factor (Part One, the six-verbs test). A prompt can contain highly unusual verbs and still produce a conventional song if its structure, genre references and arrangement remain generic. Use verbs to describe what the music *does*. Use constraints to determine what the music is allowed to *become*.

### 2.2 · The grammar in a song

Four principles from Part One, with the musical examples that taught them.

#### Specify the structure

Principle 1, architecture

Structure is the strongest control available, because clichés enter through familiar architecture. The default is intro → verse → chorus → verse → chorus → bridge → final chorus. Interrupt it by naming the architecture directly.

- No intro; the vocal begins on beat one.
- The first section contains no repeated line.
- The chorus appears only once.
- The second verse is shorter than the first.
- The bridge arrives before the second chorus.
- End immediately after the first complete refrain.
- Do not resolve the final chord.
- Use an instrumental interruption instead of a conventional bridge.
- Allow the song to end during an unfinished phrase.

> **Requests originality:** Make the structure unconventional.
>
> **Makes familiar solutions unavailable:** Begin with a bare vocal phrase on beat one. Add one instrument in each section, each section fuller than the one before, then strip everything back to percussion. Introduce the only full chorus near the end and stop on an unresolved IV chord.

#### Introduce contradiction and tension

Principle 2, contradiction

Systems perform predictably when descriptors point the same way. “Warm,” “organic,” “acoustic” and “intimate” form a familiar cluster. Unusual results emerge when instructions pull against one another.

- Bluegrass instrumentation at drum-and-bass tempo.
- A childlike melody over funeral pacing.
- A dry, close vocal above a huge, distant rhythm section.
- A danceable bass line under lyrics that never resolve emotionally.
- Medieval modal harmony with a cheap 1980s drum machine.
- A lullaby delivered with the timing of a courtroom statement.
- Delicate instrumentation played with mechanically perfect repetition.

The aim is not random absurdity. The elements should create productive tension. Ask: which element should feel human, and which mechanical? Should the lyrics contradict the harmony, the rhythm, or the delivery? Where should the listener feel instability?

The formula

    Familiar element A
    + incompatible element B
    + one specific execution rule

For example: use a gentle folk melody with industrial percussion, but keep the vocal completely calm while the rhythm becomes increasingly aggressive.

#### Use narrow references, not broad genres

Principle 3, narrow reference

Genre labels are too large to be useful. “Rock,” “ambient,” “soul” and “cinematic” each lead to thousands of predictable combinations. A narrow reference points to a smaller musical neighbourhood.

- The dry drum sound of a late-1970s Tokyo studio.
- A one-microphone room recording with audible chair movement.
- The harmonic restraint of an early demo rather than a finished album.
- A regional dance rhythm played by a small acoustic ensemble.
- A field recording beneath a nearly silent vocal.
- The brittle synthesiser tone of low-budget television music.
- A live rehearsal where the musicians are uncertain of the arrangement.

A good reference identifies several dimensions at once: period, place, recording environment, instruments, performance style, production limitation. Describe a specific sonic situation, not a famous artist or a broad genre.

#### Use negative space to remove defaults

Principle 4, negative space

Systems add things you never asked for. Naming them and forbidding them is often more effective than describing what you want.

- ~~a conventional intro~~
- ~~atmospheric pads~~
- ~~large reverberation~~
- ~~stacked harmonies~~
- ~~cinematic strings~~
- ~~a key change~~
- ~~a final chorus repeated several times~~
- ~~a drum fill into every chorus~~
- ~~background vocal responses~~

A strong prompt pairs a positive instruction with a prohibition: *use a single dry vocal over sparse percussion; no pads, no harmonies, and no reverb until the final section.*

Do not ban everything. Excessive prohibition makes results thin or incoherent. Select the defaults that conflict most with your intended character.

Ban things, not qualities. “No harmonica” removes a harmonica. “No emotion” or “never spoken” names the very manner you want gone, and the system tends to supply it. For delivery, describe what you want instead.

### 2.3 · Treat the lyrics as a control surface

Lyrics are not words placed on top of a melody. Their shape influences phrasing, rhythm, melodic contour and breathing.

#### Irregular line lengths

Regular lines encourage regular phrases. Uneven lines encourage the vocal to shift between clipped and extended delivery.

    I carried the cup
    through the room
    where nobody had asked me to stay

#### Unexpected stresses

    I said the window was OPEN
    but meant the opposite

#### Enjambment

Let a thought run across a line or section boundary. The incomplete phrase creates a natural point of tension.

    You left the light on
    for someone who would only

#### Line breaks as phrasing

Many systems read line breaks as phrase boundaries. Break a sentence in an unnatural place to create a pause. Crowd syllables onto one line to rush the delivery. Use a one-word line to create space.

    I thought I heard you say
    no
    not yet

#### Performance tags

Some systems respond to tags in the lyric field more reliably than to general style instructions. Use them where they mark a meaningful change, not as decoration.

- \[whispered\]
- \[spoken\]
- \[a cappella\]
- \[breath\]
- \[unison\]
- \[off-mic\]
- \[instrumental break\]
- \[half-sung\]

    [spoken]
    The door was open.
    [whispered]
    The room was not.
    [a cappella]
    And I went in anyway.

### 2.4 · Generate in sections when possible

Whole-song generation invites familiar architecture. Section-by-section generation creates a decision point at every boundary — precisely where generic arrangements appear.

- Generate the opening section. Keep or revise it.
- Extend into the next section.
- Decide whether the arrangement should expand, contract, or change direction.
- Generate the ending separately.
- Assemble or edit the strongest sections.

Slower, and it preserves authorship over the architecture.

### 2.5 · What prompting cannot fix

Prompting strongly influences arrangement, instrumentation, section order, vocal phrasing, performance energy, the presence of harmonies, and rhythmic density.

Other characteristics are embedded more deeply: glossy mastering, excessive compression, synthetic vocal sheen, generic spatial effects, uniform loudness, overly polished timbres.

If the arrangement is strong but the sonic fingerprint remains obvious, treat the output as **source material, not a finished recording**. Export stems. Replace the vocal. Replay selected instruments. Resample through your own effects. Record room ambience. Reshape the reverb. Rebuild parts with real instruments.

Use AI for rapid sketches, unusual combinations and structural experiments; use human performance and production to create identity.

### 2.6 · Expand the reference pool

Specific references only help if the references themselves are varied. If every reference point comes from major commercial releases, the system stays in commercial territory.

- Field recordings and regional musical traditions.
- Local scenes, early demos, rehearsal tapes.
- Incomplete arrangements and non-Western song structures.
- Amateur recordings and unusual instrument pairings.
- Obsolete recording technologies.
- Live performances with audible limitations.

The goal is not to imitate any one source. It is to give the system access to less commonly combined characteristics.

### 2.7 · Test whether the result is actually fresh

Novelty is easy to misjudge. Something can feel original simply because you have not recently heard what it resembles. Play the draft for someone with deep listening experience in the style; they may recognise a familiar melodic contour, a borrowed rhythmic gesture, a standard arrangement template, a production cliché.

The question is not whether the piece has never existed in any form — that standard is impossible to prove. The useful questions are narrower:

- Does the combination feel personally chosen?
- Does the arrangement avoid the most obvious template?
- Does it contain at least one decision that could not be predicted from the genre label alone?
- Does the unusual element serve the lyric, rather than advertise its own strangeness?

### The prompt template

    Create a song built around the following constraints:

    1. Structure
       [Section order, entrances, repetitions, ending.]

    2. Main contradiction
       [Two elements that pull against each other.]

    3. Narrow reference
       [A time, place, recording environment, instrument,
        or production limitation.]

    4. Vocal behaviour
       [Phrasing, timing, register, breath, delivery, restraint.]

    5. Negative space
       [Two or three defaults that must not appear.]

    Do not add a conventional intro, a key change, a repeated
    final chorus, or unnecessary background harmonies.

Worked example

    1. Begin with the vocal on beat one. One verse, one instrumental
       interruption, and one chorus that appears only once. End before
       the final phrase resolves.

    2. Combine a childlike melodic contour with funeral pacing.

    3. Use the dry drum sound of a small late-1970s studio and the
       limited room ambience of a one-microphone rehearsal recording.

    4. Keep the vocal almost conversational in the verse. Let it become
       strained only on the final two lines.

    5. No pads, no vocal harmonies before the closing chorus, and no
       orchestral strings.

    Favour tension, restraint and incomplete resolution over polish.

### The working method

- **Define the architecture.** Decide what the song will not do structurally.
- **Choose one contradiction.** Pair two musical ideas that create useful tension.
- **Select one narrow reference.** A specific sound, place, era, recording condition or limitation.
- **Shape the lyrics.** Line lengths, stresses, pauses and section boundaries, used deliberately.
- **Add two or three exclusions.** Remove the defaults most likely to make the result generic.
- **Generate several versions.** Treat the first output as a sample, not an answer.
- **Change one variable at a time.** Preserve what works while testing what does not (Principle 9).
- **Generate sections separately.** Keep control over transitions and endings.
- **Curate the strongest outlier.** Choose the version with the most meaningful surprise (Principle 11).
- **Finish outside the model.** Edit, re-record, resample and mix away the remaining generic qualities.

### Case study: “I love you, baby”

Specificity of constraint, applied to a finished lyric.

This isn’t a love song. It’s a portrait of a man coming apart, written in a love song’s vocabulary. She’s with someone else. He’s the affair. The evidence is in the morning: bloodshot eyes in a mirror he didn’t want to face, whisky in the good memory, and that quietly chilling line — *every thought of me without you leads to somewhere I don’t want to go.*

The lyric says *I love you, baby.* The details say *I can’t survive without you*, which is a different thing, and the writing knows it. The arrangement’s job is to side with the details over the claims.

#### The structure override

The title hook is the most clichéd phrase in all of popular music — so it gets delivered as the smallest moment in the song. Every template screams that *I love you, baby* is where the chorus lifts, the drums enter, the voice opens. Instead the band thins, and he sings it quiet, worn, almost ashamed. In this story it isn’t a declaration; it’s a man pleading at three in the morning. The verses carry more sound than the chorus. Full inversion, earned by content.

#### The setting

Last call. A worn upright piano, brushed kit, low tremolo guitar — the sound of the bar where they used to laugh over whisky, after everyone has gone.

#### The lyric, reformatted for phrasing

    [Verse 2 — lower, rougher]
    I got out of bed this morning
    didn't want to face the glass
    Saw those tired bloodshot eyes
    and memories came flooding back
    I thought about sitting with you
    laughing softly over whisky

    God
    the way you looked at me
    told me what you wouldn't say
    out loud

    [Verse 4 — barest]
    And maybe I'm a fool
    for holding on
    Maybe I should cut my losses

    But every thought of me without you
    leads to somewhere
    I don't want to go

“God” stands alone. “out loud” is broken off — what she wouldn’t say, hanging in the space where she didn’t say it. “here” is isolated at the end of verse three, because he’s insisting on a presence that isn’t present. The dark line is split across two lines inside white space, and the music hollows out beneath it: acknowledged, not decorated. Both choruses are tagged progressively smaller, the last quietest of all, so the song ends at its point of maximum need and minimum voice.

#### The style prompt

    Slow 12/8 ballad on a worn upright piano, slightly out of tune,
    with brushed drums and a low tremolo electric guitar far in the
    background, nothing else — recorded like an empty bar at closing
    time, chairs up, one light on. Male voice, hoarse and worn, close
    to the mic, singing like a man who's been up all night, phrases
    sagging slightly behind the beat. The verses carry the fuller
    sound; at every chorus the arrangement thins instead of lifting —
    drums drop to almost nothing and the title line is sung small,
    quiet, almost ashamed, a plea rather than a declaration. On the
    line about where his thoughts lead, the guitar and drums fall
    silent, leaving only a single low piano note under the voice,
    then the song resumes. The final chorus is the quietest music in
    the song. After the last line the piano keeps playing alone for a
    few bars, unresolved, like he's still sitting there, then stops.

    No guitar solo, no horns, no gospel backing vocals, no big
    blues-rock drums.

#### How the slots were filled

- **Structure override:** the hook as the smallest moment — the anti-chorus — with choruses that shrink in sequence.
- **Contradiction:** the most clichéd title in music delivered as the least triumphant sound in the set. Devotion’s vocabulary, dependency’s voice.
- **Narrow reference:** the bar at closing, chairs up, one light — the whisky memory’s location after the memory is over.
- **Performance verbs:** sags, thins, hollows, pleads.
- **Negative space:** four targeted prohibitions at the end, plus an explicit ending — the piano outlasting him.

#### Geography check

Slow 12/8 plus a hoarse voice plus a bar pulls hard toward blues-rock and toward big torch-song belting. Both are anchored against in the negatives and in the “small, ashamed” chorus instruction. If a take comes back belted anyway, the one-variable fix is to strengthen the vocal line to *never rises above conversational volume anywhere in the song.*

The anti-chorus is the bet. Keep whichever take sings *I love you baby* smallest; that delivery is the entire reading.

#### What the take taught

The anti-chorus landed where it mattered most. The final chorus is the quietest section of the song, with the drums almost gone, and the dark line flows straight into it: *somewhere I don’t want to go* and the smallest *I love you baby* sit in one continuous hollow. The first chorus held only partly. It opened on a lift before thinning, so the shrinking happened across the song rather than at every chorus.

One deviation stayed. *Say you’ll come back tonight* rises in the final chorus. The prompt didn’t ask for it, but desperation breaking through is true to him.

The ending did not obey. After the last line, the model reached for the one thing this song couldn’t have: a closing swell, the loudest moment in the whole generation. The piano outro I’d asked for came after it and couldn’t be saved without it. So I cut on his last word, *without*, and faded. Exhaustion rather than lingering, which suits him better.

**Endings are where the model most wants its climax.** Generate them separately when you can, and be ready to finish with an edit.

### Case study: “Desperate Skin”

One absolute rule, held for an entire song.

The lyric hands over its reading in the first image: the narrator is feigning sleep. Hands trembling beneath the pillow while the other stumbles in — awake, silent, unseen. So the move is total. **The whole song is sung as if not to wake someone.** Barely above a whisper, close enough to hear breath, tense and constricted — a voice that cannot rise, because rising would be discovery.

This is quiet as danger rather than quiet as tenderness. The contradiction is a lullaby’s volume carrying the ugliest content in the set.

#### The room outranks the person

The lyric scores its own soundtrack — screen door, screaming neon clock, bleeding light. The room is loud; the person is silent. So the arrangement inverts the usual hierarchy: a constant electric hum sits slightly forward, oppressive, while the instruments are skeletal. A low guitar figure. A distant piano note or two. **The room as the loudest presence, the human barely audible inside it.**

#### The lyric, formatted

    [Bridge — flattest, near-spoken]
    We died long before tonight
    back when the drinking started
    I know love turns into loneliness
    one betrayal
    at a time

    I already know the ending
    I just can't leave yet

“with you” is broken off both refrains — the trap’s last ingredient, landing separately, almost inaudible. “one betrayal / at a time” is staircased, erosion at erosion’s pace. The bridge’s two facts are isolated and stated flat, with no melody asked to carry what the voice won’t feel aloud.

#### The style prompt

    Slow airless minimal piece built on a constant low electric hum
    like a neon sign buzzing through a wall — the hum never stops and
    sits slightly too loud, oppressive — with a skeletal low guitar
    figure and a distant piano note or two, nothing else, no drums
    anywhere. Recorded suffocatingly close, like 3 a.m. in a small
    bedroom trying not to be heard. Voice barely above a whisper the
    entire song, tense and constricted, every word close to the mic,
    sung like someone feigning sleep who cannot risk being louder —
    the voice never rises, not even at the refrains, which are only
    slightly more voiced than the verses. The bridge is flattest of
    all, nearly spoken. In the outro the guitar and piano fall away,
    leaving only the hum and the whisper, and after the last line the
    hum continues alone, steady, for several seconds, then stops.

    No drums, no swells, no reverb, no full singing voice anywhere.

#### Why this is the cleanest constraint in the set

One absolute rule does all the work: *the voice never rises.* It is a ceiling rather than an arc — and unusually, it is **verifiable by listening**. Either the voice rose or it didn’t. Most craft decisions require interpretation to assess. This one does not.

The known risk was the model’s instinct to lift at the refrain, which it would face twice. The guard was comparative rather than absolute — *only slightly more voiced than the verses* — because a flat prohibition with no relative anchor tends to produce a dead delivery rather than a restrained one. The selection rule followed from that: keep whichever take stays smallest at the refrains, because a single full-voiced line breaks the feigned sleep and the spell with it.

**Geography check:** whisper plus drone pulls toward dark ambient and whisper-folk — both wanted here. The fence is against beautiful gloom, the reverb-washed prettiness of slowcore, held by “no reverb” and “airless.” This room should not sound lovely. If the hum comes back warm rather than oppressive, the one-variable fix is “harsh fluorescent buzz” in place of “neon hum.”

#### What the take taught

The finished vocal read as *resignation* rather than the tension the prompt described. That looked at first like a drift from the design. It wasn’t. The refrain names exhaustion as the mechanism of captivity — *my body’s weak, my spirit worn, that’s what keeps me trapped here.* Rage would have been the cliché rendering, and rage implies energy, and energy implies the door is usable. A voice too tired to be angry is the truthful one.

Fear is why the voice stays small tonight. Exhaustion is why it has stayed small for years. The two readings were not competing; they were the same night at different depths. **When a take diverges from the prompt, check the lyric before assuming the model was wrong.**

The ceiling held everywhere but once. On *Still wearing this desperate skin*, near the very end, the voice rises slightly, a brief flash of anger or frustration, and then resignation returns for the last three lines. The prompt forbade exactly this, and I kept it. Because the rule had held for the entire song, the one breach could not read as a mistake. It reads as the only moment the narrator almost wakes up.

The hum taught the opposite lesson. I had asked for it slightly too loud, oppressive. The take that worked keeps it barely discernible. Pushed forward, the oppression became a distraction: the listener notices the sound effect instead of the person trapped inside it. The room should press on the voice, not compete with it.

**Make the rule strong enough that a single deviation becomes meaningful.** An absolute constraint can be a song’s emotional architecture, and a small violation, placed once, can say more than perfect compliance.

### What v6 changed

Six near misses, re-made on a new model. Added October 2026, updated November 2026, from work with Claude.

When Suno v6 arrived, the verdict online was immediate: it’s worse. My first test agreed. The prompt for “Clothed in Fire,” which had given me a take I’d called a bullseye on v5.5, came back underwhelming.

Then I went back to the v5.5 take and heard what I had missed months earlier: the voice was performing, not reporting. Fully sung where it should have been level, the choruses rising where they should have stayed flat. The bullseye had been a near miss. v6 wasn’t ignoring the prompt. It was following it more literally, and the prompt was loose.

**A model that follows instructions more closely rewards the people who know exactly what to ask for, and punishes the ones who relied on its instincts.** Both can be true at once: better for directed work, worse for undirected work.

#### The rules v6 taught

- **1. Describe what is heard, not who is singing.** “A witness telling what he saw” was acted. “Controlled anger, biting off the ends of lines” produced mannerisms with no person behind them. “Singing on a narrow, level melody, reporting rather than performing, no emphasis” produced the song.
- **2. Ask for the delivery you want; don’t name the one you fear.** “Completely flat, no emotion” came back lifeless and cold. Adding “fully sung, never spoken or half-spoken” came back half-sung. Bans work on instruments (“no drum kit” held every time), but a way of singing, named even to forbid it, tends to appear. Describe the target instead: “singing on a narrow, level melody.” Where a limit is needed, lead with the positive: “half-sung on a simple melody, still pitched.”
- **3. Point at sections; don’t ask the model to find them.** “Whenever the lyric returns to the real world” made it guess, and it guessed wrong. “The third verse, the fourth verse and the outro” left nothing to guess.
- **4. Check your rules against each other.** The earlier, broader rule wins. A groove that “never stops” will not stop dead later. A voice “fully sung” throughout will not half-speak one verse.
- **5. Words cast performers.** “Chanted” brought a crowd. “A small gathering of friends” put people in the room for the whole song. And parts still add up to a genre: pedal steel plus a slow 6/8 waltz is country, whatever you call it.
- **6. Images carry tempo.** “Funeral pace” and “a waltz with the joy taken out” pulled the takes somewhere strange. “6/8 at about 60 beats per minute” did not.
- **7. Backing voices go everywhere or nowhere.** Placement rules that held on v5.5 did not hold for group voices on v6: mention a group anywhere and it sings everywhere. Leave the voices out, or control them afterwards with stems.
- **8. Remove the failing device before adding control.** Two songs were rescued by taking away the feature that kept failing, a chamber-instrument switch and a choir, and hearing that the song had never needed it.
- **9. Judge a prompt on two takes, and check what you submitted.** The same prompt gave one miss and one bullseye. And once I credited a new clause with fixing a song, when the clause had never made it into the prompt: I was hearing other takes of the old one.
- **10. Feelings aren’t a sound.** My first prompt for “Never Be One Again” named the right feelings: “slow burn, dignity over rage, exhausted heartbreak, someone trying not to break while singing.” It named no sound, so the model chose the most familiar sound of heartbreak, piano and voice, and used the piano to act out each feeling. Feelings tell the model what to express. Sounds tell it what to play. Write both.
- **11. When the words and the prompt disagree, the words win.** Eight takes refused to sing the last lines of a verse “quieter, closer.” They were the most hurtful lines in the song, and sung quieter they would not have been true. Once the tag was removed, the verse settled. If an instruction keeps failing in one place, read the words there: the model may be right.
- **12. Know when to stop generating and edit.** “One final bass note” never came back as one note in eight takes; models don’t count. I removed the request and cropped the ending by hand: last word, one bass note, a short fade. A crop is part of the work, not a failure of the prompt.
- **13. Constrain only what protects the song’s truth, and cut the rest.** The prompt for “When the Time Is Right” grew by patching until it directed every moment: where the piano spoke, how many lines were spoken, how the ending stopped. Eight takes moved me and none obeyed, and where they disobeyed, the song was right: the accounting verse was spoken, and the piano played on after the last line to leave room for reflection. Cut from 977 characters to 569, keeping only the sound, the voice and the bans, the prompt gave two strong takes in a row. The better one did two things no instruction asked for: the voice rose on only two lines of the quietest section, and the last line was half-sung in silence. Test every clause: if the model ignored it, would the song become less true? If not, cut it. A prompt that directs every moment leaves the song no room to surprise you.
- **14. Shape the song with comparisons.** Describe each section against the one before it, not on its own. For “Animal”: “each section plays slightly looser and hotter than the one before,” the bridge stripped bare, “the final chorus is the one full release.” One kind of instruction carried the whole arc.
- **15. Fence each restraint to the part it belongs to.** Absolutes travel. In “Beautiful Soul,” “he never opens up into full emotional singing anywhere” held down the one line that needed to rise, and “no build” fought a cello I had asked to swell. In “The Sun of Gods and Man,” a drone “that never stops” could not stop at the end; it became a drone “under the whole song.” Say where a restraint applies, or it applies everywhere.
- **16. Every word does a job. Make sure it’s the one you meant.** “Narration” brought a speaking voice. “Unaccompanied” (to a musician, no instruments) was read as “no other voices.” “Ends on a high note” may be taken literally. When a take does something strange, look for the word that asked for it.
- **17. Tell the voice what to do on the lines that matter.** “Every quoted line dips lower, like remembering how the words sounded” gave “The Sun of Gods and Man” its three remembered voices, each sung noticeably lower. The mother’s line was asked to go lowest of all and dipped about as far as the others: a model follows the direction of an instruction more readily than its degree.
- **18. Every “or” hands the decision to the model.** “Brushed drums or none at all” and “cello or ambient steel guitar” let the model choose, and it chose a mid-tempo country song with a steady beat. If you know what you want, choose it yourself.
- **19. Give the unspoken feeling to one instrument.** When a singer holds back, name the instrument that carries what he won’t say, and describe how it plays: “long, flowing counter-melodies around and between his lines with a full, singing tone, swelling where his voice stays level.” The voice stayed level; the cello said the rest.
- **20. A conventional description gets the most famous sound.** A second prompt for “Living a Lie,” written from the same line about the song’s meaning but in general terms (sparse, hushed, late-night), came back sounding like a famous singer. The prompt built from the lyric’s own world (a drum machine that never varies, two instruments that never meet) did not. The palette belongs to the lyric, not to the genre.
- **21. Endings need their own section, or your hand.** Models run on. Give the ending its own tag on the sheet, with nothing after it but \[end\]; crop by hand when the take overruns; or set the song’s duration so the ending has to fall inside it. A duration of three minutes gave “Living a Lie” its whispered last lines and then silence.
- **22. Hold back the one thing the song is waiting for.** For “If You Could Feel,” the harmony stays suspended for the whole song and resolves only on the last two lines, where the voice steadies. v6 held the suspense and resolved exactly where asked. A model will wait if you tell it what it is waiting for.
- **23. Regenerate, don’t rewrite.** The first take after a fix to “The Sun of Gods and Man” was flawless until the model fumbled a word. That was the model’s slip, not the prompt’s. Generate again before changing words that worked.

#### A setting worth knowing

In Suno, the magic wand beside the style box is not an on/off switch. It suggests styles when you click it, and the suggestions only enter your prompt if you add them. (It turns blue when My Taste is on, because it then draws its suggestions from your taste profile.) Personalize, which applies My Taste to the generation itself, needs Variety turned on; with Variety off, it stays off. Write your settings down with every prompt, so a result you like can be repeated.

#### The six

| Song                   | The near miss                                                                                              | What fixed it                                                                                                                                                                                                       |
|------------------------|------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Clothed in Fire        | Performed instead of reported; then, hardened to “completely flat, no emotion,” nearly spoken and lifeless | Every word for speech and every “no emotion” removed; the voice described as it should sound: “singing on a narrow, level melody, reporting rather than performing.” A ban on speaking, tried first, made it worse. |
| Crash and Burn         | Voices arrived early; the music would not stop                                                             | The early voices were right (“we’re in this together”), so they became a rule. The ending was cropped.                                                                                                              |
| My Darling, Darling    | Chamber instruments bled into the real world; the dream verse came out spoken                              | Sections named by position, one guitar under everything, the voice fenced both ways. The arrangement thinned by itself.                                                                                             |
| Indigo Soul            | Group voices in every verse                                                                                | The group removed. The take kept has one faint voice joining on a few lines, as if to say, you’re not the only one.                                                                                                 |
| Never Be One Again     | Shouting on v5.5; soulless on v6                                                                           | Prompted the grief under the anger: “hurt more than angry, the anger in the words, never in the volume,” one feeling per section                                                                                    |
| When the Time Is Right | A bad country song                                                                                         | Pedal steel and the funeral-waltz image cut; tempo given as a number; the voice described as a state, not a technique. Later, most of the arrangement instructions were cut too, and the song got better (rule 13). |

Rules 10 to 21 came from the episodes of the [Method series](https://youtube.com/@amonrosewords), where each song is shown through a beginner prompt and a precise one, on the same model. Two habits run through all of them: when a take is truer than the prompt, keep it; and when the model gets something right that you didn’t ask for, write it into the prompt so it happens again.

#### What it means

The method did not change. Read the lyric for its truth, constrain the model toward it, judge what comes back. What changed is how literally the model reads. On a looser model, a loose phrase was rescued by instinct. On a stricter one, every word is an instruction, including the words you never meant as instructions.

The fault the complaints blame on the model is often in the prompt. Not always: some ceilings are real, and endings still need scissors. But an ugly first render is the beginning of the diagnosis, not the verdict.

## Part Three · Images

The grammar was learned on songs. This part tests whether it holds for pictures, on the same terms: the same subject, prompts that differ only in how much they decide, two takes each, on two different generators.

### 3.1 · Freedom, detail, and decisions

The subject was a picture-book moment: a young girl who has lost money, crying in a park. Three prompts, each run twice on Suno’s image model and twice on ChatGPT, in fresh chats with nothing attached.

> **A · Maximum freedom:** A girl crying in a park.
>
> **B · The typical “detailed” prompt:** A beautiful, emotional children’s book illustration of a sad little girl in a red dress crying in a lovely sunny park, highly detailed, vibrant colors, heartwarming, storybook style, masterpiece.
>
> **C · Boxed in:** Children’s book illustration in flat gouache on rough watercolour paper, visible brush strokes, a limited palette of red, ochre, olive green and cream, simple dark ink outlines. A skinny girl of about seven, seen from slightly above, stands alone at the left edge of the page on a plain dirt path; her long dark braid hangs forward, and she wipes her eyes with the back of one hand while the other pulls an empty dress pocket inside out. Her face is drawn simply: small dot eyes squeezed shut, a narrow wobbly mouth, round cheeks with no shine. A wide empty lawn fills the rest of the page, with one bare wooden bench far away and a low grey sky. Quiet, lonely, still.

#### What came back

- **A, on both generators:** a photograph, not an illustration, of a young woman rather than a girl, on a park bench in autumn, with fallen leaves and grey light. Two different models, given no direction, reached for the same stock image of sadness.
- **B:** each model’s house style, and each model’s two takes nearly identical. Both added things nobody asked for. Both reached for a comfort object (a stuffed bunny, a bear, a puppy), because “sad child” plus “heartwarming” points there. One added a gazebo, a duck pond, an arched bridge, bows and frills.
- **C:** both models followed nearly every decision: the texture, the palette, the camera, the girl at the left edge, the empty pocket, the distant bench. Each model’s two takes looked like two pages of the same book, and the two models’ results looked like each other. The picture came from the prompt, not from the model.

What C left open, the models filled: both added a collar and long sleeves, and drew the camera more side-on than “slightly above.” A specific prompt still has gaps, and the gaps get the default.

> **A detailed prompt isn’t a specific one. B is the longest-sounding and the most generic: all qualities, no decisions.**

### 3.2 · Constrain the style, not only the content

This is where pictures differ from songs. Image models have a house style, glossy, softly lit, slightly three-dimensional, and adjectives of quality (“beautiful,” “highly detailed,” “masterpiece”) pull straight into it. Content decisions alone don’t escape it. Naming the medium does: the paint, the paper, the line, a limited palette, how a face is drawn.

Faces need the most care. “Cute girl, freckles” lands on the average storybook face. Concrete drawing rules move it: dot eyes, a single line for the mouth, round cheeks with no shine.

Banning a default works no better here than in music (Principle 4). Asking for a park with no gazebo can bring one in. Describe what is there instead: *a winding path between lawns, one big oak, a bench, open sky.*

### 3.3 · Say where things are, and how big

Illustrating a full picture book exposed the instructions that pictures need and songs don’t.

- **Direction is ambiguous until it’s anchored.** “He strides along the path to the right” sent a boy across the path toward the grass. What worked described the path first and then put him on it: *the path runs straight across the picture from the left edge to the right edge; he walks on it, both feet on it, heading toward the right edge.*
- **Give sizes a measuring stick.** Passers-by came back tiny until the prompt said they stood on the same sidewalk as the girl, at the same distance, so the adults stood about one and a half times her height. A distant face needs the same: *about a third of his height on the page, large enough that her open mouth is visible.*
- **Split directions explicitly.** “Shoppers walk past her” sent them all one way. “Three walk to the left and three to the right, passing each other” did not.
- **Name the format first.** “Portrait page” was ignored more than once. Opening with *vertical 2:3 portrait format, taller than wide* was not.
- **Anything left unasked comes back empty or typical.** A street with no passers-by named came back deserted. A park whose season wasn’t fixed drifted toward autumn, because autumn is the stock setting for sadness.

### 3.4 · What constraint can’t hold: a world across many pictures

Constraints control what a single image looks like far better than they control sameness across images. A song is one generation: the voice and the instruments stay consistent inside one take. A picture book is twenty-five separate generations, and each one redraws the world.

Over a full book, the characters held up better than the world: the same faces, hair and clothes, once fixed by character sheets attached to every request, though small details such as freckles still came and went. The world did worse. Objects on a market counter multiplied. A paper bag’s print changed. A dress’s pockets changed shape. The oak moved sides, the path rerouted, the sky changed colour from page to page.

Three habits narrowed it:

- **Remove the detail that keeps drifting.** Plain shorts instead of patterned ones. A closed paper bag instead of peanuts showing at the top. The same move as removing a failing instrument from a song (Part Two, What v6 changed, rule 8): if a detail can’t be held, take it out.
- **Write the fixed descriptions once and paste them word for word** into every prompt: the style block, each character, the props. Attach the first good picture of a place as the set for every later picture of it.
- **Fix with the edit tool, not by regenerating.** When a picture is right except for one thing, brush over that thing and describe the change. Regenerating the whole scene redraws everything you had right.

Even so, a printed book needed a human illustrator. The generated pictures became something else that was still valuable: a dummy showing the staging and emotional beat of every page, with the text in place, for an illustrator to work from.

> **Constraint makes one picture specific. Only a person holds a world steady across a book.**

## Finally

### The part that doesn't transfer

Everything in this manual can be taught, and most of it can be learned in an afternoon. None of it is the scarce thing.

The scarce thing is knowing, before you generate, which single moment will decide whether the work is any good — and then recognising it when it arrives in a form you did not plan. That is not a technique. It comes from caring about the material for long enough to know what it needs.

A generative system is fluent and without taste. It has no stake in the outcome, no memory of what moved you, no view about whether a line should land small. Its fluency is genuinely extraordinary, and it is not judgement, and the difference between them is the whole of the work.

Which is why the method can be given away without losing anything. The prompts were never the valuable part.

**Hold the vision.  
Supply the specific.  
Refuse the average.  
Judge relentlessly.  
Keep developing the human. The human is the ceiling.**

Constraints remove options, and removing options is the most reliable way to keep a probability-driven system away from its comfort zone. The objective is not to make a machine strange. It is to make the obvious answer unavailable, and then to recognise the unusual answer that still works.

There is a word for the arrangement this describes, and it is more precise than collaboration or partnership. **Mutualism** — two parties of different kinds, each supplying what the other structurally lacks, producing what neither reaches alone. The machine brings fluency without judgement, range without stake. The person brings vision, taste built over a lifetime, and the capacity to care how it turns out. Remove the human half and there is no mutualism, only a system averaging in the dark.

This is not a music skill, or a writing skill, or a technical one. It is the general skill of staying the author while the tools get loud — and when the next capable thing arrives, the method is the same. Constrain it. Contradict it. Generate ten. Keep the strangest. Never mistake the tool's fluency for your own judgement.

A. Monrose, with Claude. Our manual: written together, from the songs and pictures we made this way. First published November 21, 2026.

The songs this method produced, in method videos (Thursdays from November 19, 2026) and in *Made of Light* music videos, where the people in each song are drawn as figures of light, in code, by Claude under my direction: [youtube.com/@amonrosewords](https://youtube.com/@amonrosewords)

How it’s all made, and everything else: [A. Monrose](https://claude.ai/artifact/EFSmzCARp5vCo2deHnYRCg)

Free to read, quote and share. If it’s useful, say where you got it.

