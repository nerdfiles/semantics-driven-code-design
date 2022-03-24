# The Metaphysics of CSS

Consider these [mixin][mixin] names

```
.A-rolodex--container__self__ {}
.TYPE-BLOCK--ELEMENT__MODE__ {}
.TYPE-BLOCK--ELEMENT__MODE__ {
	@include thing;
	@include thing-atom-1;
	@include thing-atom-2;
	@include thing-atom-3;
	@include thing-atom-4;
}
```

As Derrida asserts, the metaphysics of presence is unavoidable, so our purpose 
here is to ensure systematic tasks in processing stylesheets is metacomputational.

## The opposition

A problem that is apparent today is the CSS "utility" framework approach which 
introduces names such as the following:

```
.\(F\)\(PARAM\) {}
.G\:PARAM {}
```

Generally "utility" frameworks attempt to preserve levels of and for a syntax 
tree such that parameterization is combined with space-delimited name scheme 
where prefixes are matched according to their need at the given level expressed 
in the non-standard metacomputational name's immanent structure for presentation.

Unfortunately, what happens with this naming pattern is that the name strings within 
the class attribute value are used as if they were definite descriptions and it is 
expected of the developer to manage the cascade in a hierarchical model. Quickly this 
becomes unscalable as complexity of the interface grows over time. What of the 
temporalization of the interface is lost as developers change hands or 
debugging becomes an issue. Our task is to make such temporalization explicit 
within a placeholder of the naming schema. Often numbers are used in a sequence 
to designate the temporalization in an ad hoc manner, but we want a specific 
placeholder formation such that we can seek within subbranched prefix hash tree 
for the relevant style properties to be made available in the mixin ensemble 
which determines the how the style will play out in the cascade.

Ideally only one mereologically complex name as sentence-subject will appear for 
the elemental name, rather than the developer takes some effort to describe the 
component on-the-fly. Names possess power and planning implications: was it 
poorly em-powered or poorly planned? "Utility" classes indicate overpowering 
of other names at the same level of description while when combined with a "No 
UML" approach, developers are encouraged to design-as-they-go. Such practice 
should be avoided as it results in low understandability in the design as it 
is regarded between collaborating developers.

From [Semantics-driven DSL Design][sdsld]:

```
week52 :: Cal String
week52 = D Dec 30 :-> (T 8 0 :-> "Work") :&: D Dec 31 :-> (T 22 0 :-> "Party")
```

Organic SASS analogues:

```
.state-(start)--[start]__simulator-running__ {}
.state-(simulator-running)--[pause]__simulator-pause|do__ {}
```

Think of the element re-cast from SDSLD combined with our ABEM naming format so applied to a reference implementation:

```
<div id="week52" 
     class="state-(start)--[start]__simulator-running__"
></div>
```

For all state diagrams, we can map:

1. `-` to `=`
2. 2. `--` to `:->` but
3. when inside parenticals `-` returns `:->`

Compare with yUML implicatures:

```
(start)[Start]->(Simulator running)
(Simulator running)[Pause]->(Simulator paused|do / wait)
...
```

We don't have to worry about `:&:` since it represents something like two 
sibling `<div>`s standing side-by-side in the DOM.

```
.TYPE-BLOCK--ELEMENT__MODE__ {
	@include TYPE-BLOCK-ELEMENT-1;
	@include TYPE-BLOCK-ELEMENT-2;
  ...
}
```

[sdsld]: https://web.engr.oregonstate.edu/~erwig/papers/SemanticDSLDesign-12.pdf "Semantics-Driven DSL Design. Martin Erwig and Eric Walkingshaw. School of EECS, Oregon State University, USA."
[mixin]: https://krasimir.github.io/organic-css/
