# bronner-ontology-design-patterns

Draft of OWL ontology and SHACL shapes for frame-based Ontology Design Patterns for the DTO (Digital Editions of Historical Travelogues Ontology).

The first draft of the ontology design patterns is described in more detail in our article “Interlinking Text and Data with Semantic Annotation and Ontology Design Patterns to Analyse Historical Travelogues” published in the journal Digital Humanities Quarterly: https://digitalhumanities.org/dhq/vol/17/3/000726/000726.html

## Ontology Design Patterns

The draft provides only a small set of FrameNet frame-based classes & properties (aligned to CIDOC CRM) in the [OWL ontology](/dto.owl.ttl) accompanied by the corresponding [SHACL shapes](/odp) as well as [SKOS knowledge organization systems](/kos) for typing travel types, transportation types, perception/observation types, etc.

### Travel Event Pattern

The Travel Event Pattern is based on the FrameNet frame [`Travel`](https://framenet.icsi.berkeley.edu/fnReports/data/frame/Travel.xml).

![UML class diagram of SHACL shapes for the Travel Ontology Design Pattern based on the FrameNet frame Travel](/dia/dto-travel-event.png "UML Class Diagram of Travel Event Pattern")

### Perception Activity Pattern

The Perception Activity Pattern is based on the FrameNet frame [`Perception_active`](https://framenet.icsi.berkeley.edu/fnReports/data/frame/Perception_active.xml).

![UML class diagram of SHACL shapes for the Perception Activity Ontology Design Pattern based on the FrameNet frame Perception_active](/dia/dto-perception-active.png "UML Class Diagram of Perception Activity Pattern")

### Commercial Buy Pattern

The Commercial Buy Pattern is based on the FrameNet frame [`Commerce_buy`](https://framenet.icsi.berkeley.edu/fnReports/data/frame/Commerce_buy.xml).

![UML class diagram of SHACL shapes for the Commercial Buy Ontology Design Pattern based on the FrameNet frame Commerce_buy](/dia/dto-commerce-buy.png "UML Class Diagram of Commercial Buy Pattern")

### Exchange Currency Pattern

The Exchange Currency Pattern is based on the FrameNet frame [`Exchange_currency`](https://framenet.icsi.berkeley.edu/fnReports/data/frame/Exchange_currency.xml).

![UML class diagram of SHACL shapes for the Exchange Currency Ontology Design Pattern based on the FrameNet frame Exchange_currency](/dia/dto-exchange-currency.png "UML Class Diagram of Exchange Currency Pattern")

## Annotation Scheme

Semantic annotation of a TEI encoded segment in a historical travelogue can be achieved by applying EARMARK (Extremely Annotational RDF Markup) annotation to e.g. a TEI element `seg` linking an excplicitly modeled travel event via FRBRoo representation and XPath expression to the text snippet documenting that event (i.e. part of the travelogue reporting about that travel event as part of the whole travel).  

![Proposal for an annotation scheme using standoff annotation with EARMARK for linking text and data](/dia/anno_fbroo_earmark.png)

