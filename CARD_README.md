# Mechanics Revisited card blueprint

This file records retrieval decisions specific to this deck. Universal rules
remain in the flashcards repository's card standard and authoring playbook; the
physics guide supplies domain-specific rules.

## Learner model

- Level: zero mechanics knowledge
- Confirmed mathematical/tool prerequisites: arithmetic, fractions and ratios,
  powers of ten, simple algebraic substitution, and reading a number line
- Confirmed subject prerequisites: none
- Capabilities this deck should produce: move from observable situations to
  explicit models, translate among representations, make predictions, solve
  quantitative problems, and evaluate whether an answer is physically credible
- Important exclusions: no physics term may appear as an unexplained premise;
  formalism must follow a concrete referent; later chapters cannot leak backward

Unconfirmed subject knowledge is not mastered. A target level describes the
destination, not permission to assume its vocabulary.

## Curriculum and prerequisite graph

```text
measurement and estimation
          |
          v
vectors -> one-dimensional motion -> planar motion
                                      |
                                      v
                              Newton's laws -> force models
                                      |             |
                                      +------+------+ 
                                             |
                                  work/energy and momentum
                                             |
                       rotation -> gravitation -> oscillations
                                             |
                                          synthesis
```

Each arrow is a permission boundary. A chapter may preview an everyday
phenomenon, but it may not require the later technical model to answer a card.

## Pilot concept-dependency ledger

| Concept or representation | Front(s) requiring it | Confirmed inbound source or first explanation | First supported retrieval | Later application | Status |
|---|---|---|---|---|---|
| mechanics | opening scope card | defined on that front with everyday examples | identify the two broad concerns | all chapters | supported |
| observation versus explanation | observation card | cup example supplies both statements | classify the statements | model evaluation | supported |
| physical quantity | quantity card | front defines measurable property and gives an example | identify number and unit | every quantitative chapter | supported |
| unit | quantity card | front explains agreed comparison standard | explain its role | all calculations | supported |
| SI | standard-units card | expanded and motivated on front | retrieve name and purpose | all chapters | supported |
| length, mass, time | base-quantity card | ordinary meanings plus examples on front | map each to m, kg, s | dimensions and mechanics models | supported |
| dimension versus unit | contrast card | both meanings and examples supplied on front | distinguish them | dimensional analysis | supported |
| prefix | prefix card | defined as a power-of-ten scale factor on front | interpret centi- and kilo- | conversion | supported |
| conversion factor | conversion card | equal descriptions and ratio-equals-one shown on front | choose/cancel units | all numerical work | supported |
| scale resolution | ruler card | smallest marked interval is visually explicit | report a reading justified by marks | uncertainty | supported |
| repeated measurement | repeated-reading card | five readings shown on front | infer center and scatter | experimental reasoning | supported |
| precision versus accuracy | comparison card | target/spread meanings introduced on front | contrast the terms | data evaluation | supported |
| measurement uncertainty | uncertainty card | interval interpretation introduced on front | interpret value ± uncertainty | all experimental values | supported |
| significant digits | reporting card | described as communication about resolution | reject unjustified digits | calculations | supported |
| dimension symbols M, L, T | notation card | mapping provided on front | translate quantity to symbol | consistency checks | supported |
| dimensional consistency | rectangle example | dimensions of length and area given on front | reject incompatible expression | later equation checks | supported |
| order of magnitude | powers-of-ten card | nearest-power meaning defined on front | classify 600 | estimation | supported |
| Fermi estimate | heartbeat problem | method described before name is retrieved | decompose an estimate | scale checks | supported |

Rejected from the pilot: definitions of velocity, acceleration, force, energy,
momentum, Newton's laws, free fall, and dimensional derivation of a fall-time
formula. Each depends on a later chapter. Also rejected: isolated trivia about
the labels *law*, *theory*, and *falsifiability*, which does not directly enable
the mechanics learning path.

## Retrieval portfolio

The pilot schedules these distinct decisions:

- explain why a measurement needs both a number and a unit;
- map the three mechanics base quantities to SI units;
- distinguish quantity, dimension, and unit;
- perform conversions by multiplying by a ratio equal to one;
- read scale resolution and interpret repeated readings;
- contrast precision with accuracy and interpret stated uncertainty;
- report results without invented digits;
- translate statements into M/L/T dimensions and check compatibility;
- classify a scale by a power of ten and construct a decomposed estimate;
- evaluate every numerical answer for units, scale, and justified precision.

Likely interference pairs are handled by explicit contrasts: dimension/unit,
accuracy/precision, exact count/measured value, and necessary/sufficient checks
of an equation.

## Chapter design ledger

| Chapter | Retrieval targets | Basic-card roles | Cloze candidates | Problem progression | Representations and figure opportunities |
|---|---|---|---|---|---|
| 01 foundations | measurement, SI, conversion, uncertainty, dimensions, scale | explanation, contrast, translation, misconception | stable mappings and compact invariants after explanation | identify -> convert -> read -> check -> estimate | segmented metre, ruler resolution, repeated readings, logarithmic scale: include because each tests a different representation |
| 02 vectors | scalar/directional distinction, addition, components | label, translate, compare | notation after meaning | arrows -> components -> relative direction | arrow diagrams and component triangles essential |
| 03 kinematics 1d | position, displacement, velocity, acceleration, graphs | definition, graph translation, prediction | sign conventions | qualitative -> single-step -> graph synthesis | motion diagrams and x/t, v/t, a/t graphs essential |
| 04 kinematics 2d | component independence, projectiles, relative motion | translate, predict, compare | component relations | components -> projectile -> relative motion | trajectories and paired component graphs essential |
| 05 Newton's laws | interactions, system choice, net force | causal explanation, misconception, model choice | law statements after models | interaction inventory -> free-body diagram -> dynamics | system boundaries, interaction pairs, free-body diagrams essential |
| 06 forces | common force models and conditions | discriminate and apply | model forms after concepts | isolated forces -> combined models | contact geometry, springs, friction, drag diagrams essential |
| 07 work-energy | work, kinetic/potential energy, accounting | causal, compare, translate | accounting relation | bar charts -> paths -> multi-stage | energy bar charts and force-position graphs essential |
| 08 momentum | impulse, momentum, isolation, collisions | causal, before/after, model choice | impulse relation | impulse -> 1d collision -> 2d collision | before/after and impulse graphs essential |
| 09 rotation | angular variables, torque, inertia, angular momentum | analogy, contrast, prediction | mappings after meaning | kinematics -> torque -> rolling | lever arms, rotational diagrams, graphs essential |
| 10 gravitation | inverse-square model, field, orbit, energy | predict, compare, explain | model forms | local weight -> field -> orbit | field diagrams and orbital geometry essential |
| 11 oscillations | restoring behavior, phase, energy, resonance | translate, predict, contrast | period relations | qualitative -> graphs -> driven response | phase-linked graphs and state diagrams essential |
| 12 synthesis | model selection, multi-model solutions, evaluation | discriminate, plan, debug | none planned: retrieval is strategic | scaffolded cases -> mixed unfamiliar cases | figures chosen per problem, not by quota |

## Initial-learning path

New cards are ordered so that each unfamiliar term is defined or made concrete
on a front before a later card asks for unsupported recall. The sequence is:

1. start from observable everyday situations and measurable questions;
2. attach numbers to agreed units;
3. practice the three SI quantities needed throughout mechanics;
4. convert equivalent unit descriptions;
5. inspect instrument resolution and repeated readings;
6. express uncertainty and avoid false precision;
7. use dimensions as a type-check for relationships;
8. estimate scale before trusting detailed arithmetic.

Answers refine and correct reasoning, but no answer is treated as the learner's
first exposure to a prerequisite. The completed cold-start simulation is stored
at `.flashcards/audits/pilot-cold-start.md`.

## Figure policy

Figures are original responsive SVGs with a `viewBox`, title, description,
high-contrast labels, and shape/position cues that do not rely on color. Setup
figures belong on fronts; answer-revealing annotations stay in answers.

The pilot uses four figures because they require four distinct acts: translate
equivalent units, read a marked instrument, interpret repeated observations,
and locate a value on a logarithmic scale. Decorative figures are omitted.

## Sources and accuracy

Authoritative sources, terms, access dates, and scope decisions are recorded in
`README.md`. Introductory significant-figure rules are presented as reporting
conventions, not as a substitute for an uncertainty analysis.

## Validation gate and pilot reconciliation

Before handoff:

1. run `flashcards deck stabilize . --check`;
2. run `flashcards deck validate .`;
3. inspect every changed figure at phone width;
4. reconcile planned versus actual card types, problems, and figures;
5. run `git diff --check` and review the complete diff;
6. summarize additions, omissions, and unresolved uncertainty.

Pilot plan: explanatory and contrast Q/A cards, a small number of supported
clozes, applied problems, and four functional SVGs. Pilot actuals are recorded
after validation in `.flashcards/audits/pilot-cold-start.md`.
