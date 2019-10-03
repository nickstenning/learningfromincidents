# Learning from Incidents

This repository contains links to resources mentioned in a conference talk on
**how to learn more effectively from incidents**. I most recently gave this
talk at [SREcon 2019 EMEA] in Dublin.

This talk was co-written and originally co-presented with [Jessica
DeVita](https://twitter.com/ubergeekgirl). Most of the meaningful insights in
the talk are hers, and all of the typos and errors are mine!

> If you're looking for something to do after the talk, we recommend reading
> the [Etsy Debriefing Guide], particularly pp. 21-23, which give examples of
> good questions to ask in post-incident reviews.

[SREcon 2019 EMEA]: https://www.usenix.org/conference/srecon19emea/presentation/stenning
[Etsy Debriefing Guide]: https://aka.ms/etsydebriefing

## Contents

  * [References](#references)
  * [Recommendations](#recommendations)
  * [Further reading/viewing](#further-readingviewing)
  * [Even more!](#even-more)

## References

The two links referenced in our talk were:

- [How Complex Systems Fail](https://aka.ms/csfail) is a short paper which
  focuses on how complex systems differ from the linear engineered systems we
  may have worked on in the past.

- [The Etsy Debriefing Facilitation Guide](https://aka.ms/etsydebriefing)
  contains specific guidance on how to run better post-incident reviews (which
  the authors call "debriefings".)

## Recommendations

What follows are a series of recommendations for running better post-incident
reviews and learning more from incidents.

> You shouldn't attempt to adopt all of these practices at once for every
> incident! Start small with _interesting_ incidents, and not necessarily your
> _biggest_ incidents.

We recommend that you break up your post-incident learning process into the
following stages:

1. (Optionally) interview participants
2. Run a facilitated post-incident review
3. Run a separate meeting to plan repair items
4. (Optionally) Publish written incident reports

### 1. Run a facilitated post-incident review

   At most a few days after an incident, get as many people as possible who
   were involved in incident response into a room together to talk about what
   happened.

   Have a neutral facilitator whose job it is to guide the discussion. They
   should not have been involved in incident response themselves, if at all
   possible.

   **Focus on reconstructing the timeline of the incident and understanding
   how actions and decisions of operators made sense to them at the time**,
   even if we know in hindsight that they were mistakes.

   Limit your post-incident reviews to 60-90 minutes. You will probably have
   to pick and choose what to talk about.

### 2. Use 1:1 interviews for complex incidents

   For many incidents, making effective use of a 60-90 minute incident review
   meeting will be challenging unless the facilitator already has some idea
   of the incident timeline.

   **Use 1:1 interviews (often no longer than 10-15m each) with people
   involved in the incident response to ask about their experience of the
   incident.**

   Use your interview notes to look for interesting points in the timeline:
   points where hypotheses were formed or changed, when significant actions
   or decisions were taken, or where individual views on the situation
   diverged one from another.

### 3. Keep discussion of repair items separate

   Including discussion of repair items in the main post-incident review
   meeting will make it difficult to keep focus on understanding what
   happened during the incident.

   You will likely find that talking about repair items leads people to start
   discussing what *didn't* happen. This is fine in a meeting about possible
   repairs, but it doesn't help us learn from what *did* happen.

   **Have a separate meeting a day or two after the post-incident review, in
   which you discuss and agree upon repair items.** This meeting can be
   shorter and include fewer people (typically those who have a say in
   prioritisation).

### 4. Publish written incident reports

   Not everyone on your team will attend every post-incident review. Writing
   up reports (even on one or two pages) can provide a way for the rest of
   your team to share in what was learned.

   It may make sense to prepare different documents for different audiences.
   Your immediate team may gain more from a detailed description of how the
   system surprised you. Your management chain may be more interested in
   understanding how repairs will reduce the customer impact in future.
   **Don't be afraid to prepare to different documents for different
   audiences.**

## Further reading/viewing

If you're interested in learning more about this field, here is a curated
selection of further references:

### Practical guidance

- [USDA Forest Service Learning Review
  Guide](https://aka.ms/usdalearningreviews): a guidebook for learning reviews
  conducted by the USDA Forest Service. Much of the content in this guide is
  applicable to our industry as well.

### Accessible research

- [The Field Guide to Understanding 'Human
  Error'](https://www.oreilly.com/library/view/the-field-guide/9781317031833/)
  ([Amazon](https://www.amazon.com/Field-Guide-Understanding-Human-Error/dp/1472439058))
  is a short and accessible introduction to how "human error" is a
  problematic concept in incident investigations.

### Deeper research

- [Reconstructing human contributions to accidents: the new view on error and
  performance (Dekker,
  2002)](https://www.sciencedirect.com/science/article/pii/S0022437502000324)
  is a paper which investigates how human contributions to accidents are
  often "reconstructed" during an accident investigation in ways that are not
  conducive to learning or preventing future accidents.

- [Behind Human
  Error](https://www.amazon.com/Behind-Human-Error-David-Woods/dp/0754678342)
  is a collection of papers covering the latest research into human factors
  in incidents and accidents.

### Videos

Some people learn better from videos! Here is a collection of talks and
educational videos which may be of interest:

- ["Who Destroyed Three Mile Island?" (Nickolas Means at Lead Dev London 2018)](https://www.youtube.com/watch?v=hMk6rF4Tzsg)

- ["Life After Human Error" (Stephen Shorrock at Velocity Europe 2014)](https://www.youtube.com/watch?v=STU3Or6ZU60)

- ["How Complex Systems Fail" (Richard Cook at Velocity 2012)](https://www.youtube.com/watch?v=2S0k12uZR14)

## Even more!

Here's a [further introductory guide to resilience engineering for the
software community](https://github.com/res-eng/resilience-for-software) put
together by [Lorin Hochstein](https://twitter.com/lhochstein) and [Jacob
Scott](https://twitter.com/jhscott).

If your thirst for knowledge is _still_ not quenched, you will find an
enormous quantity of research and writing on this topic assembled by Lorin in [his `resilience-engineering` repository](https://github.com/lorin/resilience-engineering/blob/master/intro.md).