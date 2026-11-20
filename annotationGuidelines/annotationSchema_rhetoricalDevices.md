# Overview

This schema defines how to annotate **rhetorical devices** in conference interpreting speeches. It provides annotation rules and their corresponding labels. For each category, examples are provided in both English and French.

# Annotation schema

We annotate two types of rhetorical devices: **humour** and **metaphors**. Humour is categorised further into irony and wordplay; metaphors are categorised as live metaphors, metaphorical concepts, or dead metaphors. For each subcategory, examples in both English and French are provided along with the device spans that should be labelled.

**IMPORTANT REMARK**: If a given phrase includes both types of rhetorical devices (e.g., a metaphor that carries irony), only the annotation for the **metaphor** should be recorded.

## Humour

### Irony (RH_HU_IR)

- Definition: a pragmatic device in which the intended meaning contrasts with the literal meaning
- Examples:

	| Language | Context | Device Span |
	|----------|----------|-------------|
	| English | I can tell you're all itching to find out the answer! | itching to find out |
	| English | So in the end, this system leaves children starving and pushing the environment to its breaking point. As if that's not a success. | As if that's not a success |
	| English | People dancing and singing, and occasionally — very occasionally — regretting their life choices the next day. | very occasionally |
	| French | Vous aussi, vous adorez quand votre train a une heure de retard ? | vous adorez quand votre train a une heure de retard ? |
	| French | Il n'y a ni nourriture, ni soleil, ni amis. Bref, c'est le paradis sur terre. | c'est le paradis sur terre |
	| French | Interdire les casques de vélo sur la route, voilà encore une idée géniale de la part des autorités. | une idée géniale |

### Wordplay (RH_HU_WP)

- Definition: the playful use of words, especially of verbal ambiguities
- Examples:

	| Language | Context | Device Span |
	|----------|----------|-------------|
	| English | This vacuum cleaner may be equipped with the latest technology, but it really sucks. | it really sucks |
	| English | Since the 2010s, asthma medication is being developed at a breathtaking pace. | at a breathtaking pace |
	| English | Obesity rates in the United States crush records each and every year. | crush records |
	| French | Malgré le bruit de la rue, mes parents s'entendent bien. | mes parents s'entendent bien |
	| French | Il va de soi que dans un cabinet comptable, chaque employé compte. | chaque employé compte |

## Metaphors

**IMPORTANT REMARKS**:
- Similes should never be annotated as metaphors. Unlike metaphors, similes make the comparison between two entities explicit through a comparison marker (e.g. "like" and "as" in English; "comme", "tel(le)", and "ainsi que" in French). However, the presence of such a marker alone is not sufficient grounds for exclusion. Fixed expressions containing comparison markers (e.g. "to know something like the back of one's hand" or "dormir comme une souche"), however, are annotated according to their respective category (see below).
- Expressions referring to living organisms (people, animals, but also plants) should **not** be annotated as metaphors (e.g., a plant being described as the biggest *enemy* or *ally* of something).

### Live metaphors (RH_MT_LV)

- Definition: novel, newly invented metaphors where the transfer from the source to the target domain triggers semantic conflict
- Examples:

	| Language | Context | Device Span |
	|----------|---------|-------------|
	| English | During the financial crisis, the company pivoted so hard it pulled a hamstring. | pivoted so hard it pulled a hamstring |
	| English | The apprentice's confidence was a full-court press the rest of the employees hadn't prepared for. | a full-court press the rest of the employees hadn't prepared for |
	| English | The city exhaled its commuters every evening through a non-stopping line of trains and buses. | exhaled its commuters |
	| French | La startup a fait un tête-à-queue sur l'autoroute de la croissance. | fait un tête-à-queue sur l'autoroute de la croissance |
	| French | Leur partenariat économique s'est fracturé comme un os sous trop de pression fiscale. | s'est fracturé comme un os sous trop de pression fiscale |
	| French | Il a dribblé les objections du conseil d'administration une par une. | dribblé les objections |

### Dead metaphors (RH_MT_DD)

- Definition: metaphors where the transfer from the source to the target domain does no longer trigger any semantic conflict. The figurative, metaphorical meaning has been fully lexicalised and can be considered (one of) the primary meaning(s) of the expression. Single-word dead metaphors are referred to as **catachreses**; multiword dead metaphors are called **idioms**.
- Examples:

	| Language | Context | Device Span |
	|----------|----------|-------------|
	| English | Make sure you don't bite off more than you can chew. | bite off more than you can chew |
	| English | Fortunately, we don't have to wait quite so long to let our hair down. | let our hair down |
	| English | The president temporarily resided in the other wing of the building. | wing |
	| French | Après un divorce, quitter sa maison peut être difficile, mais c'est parfois nécessaire pour tourner la page et oublier les mauvais souvenirs. | tourner la page |
	| French | Tout comme sa mère, Louis a déjà le sens des affaires. Les chiens ne font pas de chats. | les chiens ne font pas de chats |
	| French | Surtout si ces idées vous rongent l'esprit depuis des années. | rongent |

**TIP**: To decide whether a phrase is an idiom or not, you can consult (lexicographic) reference works.

**IMPORTANT REMARKS**:
- Idioms that do not contain any metaphorical element (e.g., "that is to say" and "last but not least" in English; "rien n'est moins vrai" and "il est grand temps" in French) should **not** be annotated as metaphors.
- Verbal expressions for which no clear non-metaphorical counterpart exists anymore (e.g., "to spend time" and "to address an issue" in English; "poser un risque" and "tomber enceinte" in French) should **not** be annotated as metaphors.
- Idioms where a minor, creative change was made to the original formulation (e.g., "let our curly hair down" in English; "les petits chiens ne font pas de chats") should still be annotated as dead metaphors, **not** as live metaphors.

### Metaphorical concepts (RH_MT_MC)

- Definition: metaphors that fall in between live and dead metaphors because they share characteristics with both types. They possess a certain logical consistency (thanks to which no real semantic conflict is triggered) but are also projective in nature.
- Examples:

	| Language | Context | Device Span |
	|----------|----------|-------------|
	| English | During the board meeting, we laid the foundations of the new company policy. | laid the foundations |
	| English | We need to pinpoint the problem before we can prescribe a solution. | prescribe a solution |
	| English | The negotiators managed to bridge the gap between the two parties. | bridge the gap |
	| French | Il faut cultiver cette relation si on veut qu'elle soit lucrative. | cultiver cette relation |
	| French | La crise a érodé les fondations de leur accord commercial. | érodé les fondations |
	| French | L'entreprise cherche à tracer une nouvelle trajectoire après ces années de turbulences. | tracer une nouvelle trajectoire |
