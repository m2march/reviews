# Comments for Author

Disclaimer on the reviewer: I currently have limited knowledge on neuroanatomy,
limiting my ability to properly judge the appropiateness of some analysis
decisions, such as the selected networks for the CPM analysis or the specific
tracts to analize through FBA. My strengths rely on knowledge of rhythmic task,
rhythmic cognition and mathematical models (in the context of this paper:
entropy calculations, ITI ratio classification, proper implementation of the
data-driven CPM approach).


# General review

### What are the major claims of the paper? 

The paper looks at whether there are structural features in the brain's
conectivity that relate to human's tendency to simplify auditory rhythms
(particularly to isochrony and simple ratios). They do so by looking at
individual differences in the proclivity to simplify rhythms and the
relationship with individual's brain imaging. Particularly, they looked if
specific brain connectivity patterns obtain via Connectivity predictive
modeling (CPM) and if differences in white matter in specific tracts obtained
through fixel-based analysis (FBA) correlated with the behavioral measures.

They found that CPM could only predict individual reduction of entropy. This
prediction was mostly driven by connections between the dorsal attention
network (DAN) and the default mode network (DMN), and between basal 
ganglia-thalamus (BG-TH) and the auditory network (AN). In particular,
participants who decreased entropy more in their response, displayed reduced
anti-correlated activity between DAN and DMN, and increased BG-TH-AN
connectivity. The paper associates this reduced anti-correlated activity with 
difficulty with task switching and attention management, which in turns
increases reliance on the BG-TH circuit to process timing, therefore being more
influenced from internal cues for timing processing. That, in turn, leads to
the simplification of the rhythms through inner rhythmic priors.

They also found changes in fiber density in two key subcortical-cortical motor
pathways correlated with increased isochrony during reproduction. The paper
proposes that enhanced connectivity within the
cortico-basal-ganglia-thalamo-cortical (mCBGT) circuit enhances propagation of
internally generated oscillations that bias motor reproduction towards
isochrony.

###  Are they novel and will they be of interest to others in the community and
the wider field? 

The paper contributes with novel evaluations of the relationship of brain
structures on the manifestation of different degrees of cognitive biases in
music processing. To my knowledge, previous work has extensively looked at
which brain areas and brain connectivity make rhythm perception, but little
work has looked at the association with biases and individual differences. As
such, it brings new information to the table that will be appreciated by the
community.

### Is the work convincing, and if not, what further evidence would be required
to strengthen the conclusions? 

I believe the conclusions can be properly derived from the analysis results. 

### On a more subjective note, do you feel that the paper will influence
thinking in the field?

The paper brings to the table the idea of looking at brain structure for the
understanding of congnitive biases. I believe this to be a positive addition to
the body of research understanding these cognitive biases. This paper provides
initial steps to understand which of these biases are more innate, and which
are acquired over time and become solidified in brain function.

# Detailed comments

## Abstract
* l.32 when talking about "increased rhythmic predictability", it is not
  completly clear what this refers to. I understand it refers to the
  "predictable motifs" explaiend in the previous sentence. I'd clarify that the
  increased rhythmic predictability is of the reproduced rhythms. 

## Intro

* l.49: it is not clear what "single reproduction means". This seems to
  contrast the iterative methodologies mentioned later. Moreover, the text says
  that "regularization tendencies" (this term could also work for the abstract
  and be used repeatedly during the text), are difficult to detect in these
  paradigm. Yet, this paradigm seems to be the one used in this experiment to
  detect the "regularization tendencies". Justification should be provided in
  the text on why the methodology was chosen despite not yielding strong
  results.
* l.52: the biases in rhythm reproduction mentioned in this paper have been 
  studied cross-culturally, showing that different cultures have different
  biases (see reference 5, 6 in the paper). There is little reference of these
  cultural differences in the introduction.
* l.53: remove 'and' after 'low entropy'
* l.82: "increase in rhythmic features" in ambiguous

## Results
### Behavioral
* A clarification for the statistical test used to validate systematic biases
  was not provided. The method section mentions an ANOVA, but provides no
  details of the tests reported on results section (l.141-147). 
* l.148: the concept "predictable patterns" is used again. I believe this 
  concept should be more properly defined, at least in the context of the paper
  (reduced entropy, increased isochrony, larger presence of specific ratios).
  In l.153 the term "rhythmic regularities" is again used. These seem to be
  used interchangably, but never made explicitly equivalent (or not) in the
  text.
* The segway into the next section at the end of the current is very good.

### Functional network interactions
* Given the novelty of the CPM method, I recommend clarifying how the method
  works. Specifically, the fact that the CPM method outputs predicted values
  of the target metric from the conectivity data between brain areas. This is
  important for the first sentence in l.176.
* During the explanation of these results, some further details or proper
  direction to the methods section is important. For example, the first
  paragraph talks about "10 canonical brain networks" (l. 172), but then in
  refers to 27 edges (l. 179). This is clarified in methods given that 84 nodes
  are used in the analysis and then reduced to the networks. 
* No reference is given to Fig 3.b. The correlations to task data mentioned (l.
  178, 186) only refer to the supplementary data.
* l. 182, it is not clear what are the statistics used to evaluate the number
  of edges between networks as being greater than chance.
* l. 185: there is no reference that k = 10 refers to 10-fold cross validation. 
* l. 185 references to figure S4, where participants are divided into two
  groups. There is no reference of what this division is and how it was made. 
* l. 207: the ending of the section could benefit from a more clear
  explanation on how the lack of anti-correlation between DMN/DAN, and
  therefor the enhanced recruitment of the BG-TH-AN circuit results in higher
  regularization.

## Discussion
* I would suggest to add discussion on how entropy can be lowered without 
higher ternary/binary/iso ratios. From how the rhythm measures are introduced
(more predictive rhythms/regularization), it sounds that they are all quite
related. Yet, the results show that these are predicted/related indepdently to
brain functioning. A debate on how these metrics differ and why some would be
represented in the brain and not others would complete the article.


## Methods

In general, in the Methods section, references are cited with text, instead of
the superscript. As a consequence, there are some citations that don't have the
full reference:
* l.336
* l.368
* l.393

Also, when referencing to the supplementary materials, I would add a detail
saying what is further explained there (e.g.: l.336, l.347).

### Experimental design

It is not clear how the sessions are divided. In general, I understand that
rs-MRI happened in one day, and all behavioral in a different one. But given
how the paragraph is written, it becomes less clear. In l.341 it says "The MRI
session [...], after which they completed [...]". It sounds like it's on the
same day to me. 

l.341 mentions other tasks which are not mentioned in the rest of the paper at
all (WAIS-IV and MET). I believe they should be mentioned. Also, reference for
the version of the WAIS-IV and MET rhythm subtest should be provided.

### CPM

I would add a bit more clarification about the 50 iterations and how they work
with the 5-fold cross-validation. I believe the explanation is clear, but I
would suggest reinforcing the difference with the process described in the
original (and cited) CPM paper (Shen et al. 2017). Mainly is the fact that the
5-fold cv is done within the 50 iterations, but there are two crossings from
the inner loop (cv) and the outer loop (50 iterations). If my understanding is
correct, you calculate significant connections for each of the 5 * 50 folds and
only use the ones that are significant in all of them (first crossing, from
inner loop to outer loop). Then, only these significant correlations on all 250
folds are used in the training process within each fold with the training data
of that fold to later predict the test data of that fold (second crossing, from
outer loop to inner loop). Finally, the predicted values for each participant
and task are average across the 50 iterations.

I also struggle to understand the preparation for the network analysis. In l.
417 it states "This approach quantifies the functional coupling between
distinct brain systems." This is done by looking at "degree-based analyses". My
understanding is that this is a graph approach, as shown by Fig. S3a. In that
case, it is not clear what the nodes of that graph is (is it networks, or the
nodes of the 86x86 matrix of the CPM?) and how the connections are obtained
from the folds vs. the 50 iterations. 

### Other

* l.401: "sopra" should be "supra"
* l.409: "severan" should be "several"


## Supplementary

### Rhythm metrics
* Shannon entropy equation cannot be read

### Figures
* Fig S1: recommendation to use bar plot instead of pie plots as they are
  easier to read.
* Fig S3: referes to the Limbic network (LIM) as light green, but in the plot
  it looks yellow.
