# Overview

This schema defines how to annotate **numbers** in conference interpreting speeches. It provides annotation rules and their corresponding labels. For each category, examples are provided in both English and French.

Numbers in written speeches can be written in digits or spelled out. We categorise numbers as either **easy** or **difficult** based on how complex they are **in speech**. In other words, we do not take into account the number of digits. Labels can differ according to the speech language, because some numbers are pronounced differently (i.e. require more vs. fewer lexical items when pronounced).

# Annotation schema

## Easy numbers (NUM_EASY)

- Definition: numbers that are simple to process when spoken, based on the number of lexical items required for pronunciation.
- Criteria:
	- integers requiring **1-2 lexical items** to pronounce
	- **dates**, regardless of their number of lexical items in speech
- Examples:
	- English:
		- 5 or "five" (1 item)
		- 27 or "twenty-seven" (2 items)
		- 2000 or "two thousand" (2 items)
		- 1959 || 2007 (dates)
	- French:
		- 3 or "trois" (1 item)
		- 80 or "quatre-vingt" (2 items)
		- 6.000.000 or "six millions" (2 items)
		- 1863 || 2025 (dates)
- Exceptions:
	- The number 1 in written form ("one", "un", "une") should not be annotated as a number since it is difficult to consistently distinguish whether it is intended as a quantity marker or as an indefinite article (esp. in French). Furthermore, this number is not typically associated with increased processing difficulty in interpreting.
	- Ordinal numbers are only annotated as numbers when they directly modify a noun. Standalone ordinals or discourse markers are not annotated as numbers (e.g. "Third, we will discuss ..."). Ordinals are not considered a separate category, but simply annotated as either easy or difficult depending on their number of lexical items.
	
## Difficult numbers (NUM_DIFF)

- Definition: numbers that are difficult to process when spoken, based on the number of lexical items required for pronunciation.
- Criteria:
	- integers requiring **3 or more** lexical items to pronounce
	- all **decimal** numbers
- Examples:
	- English:
		- 365 or "three hundred sixty-five" (3+ items)
		- 2306 or "two thousand three hundred six" (3+ items)
		- "hundreds of thousands" (3+ items)
		- 2.13 (decimal)
	- French:
		- 81 or "quatre-vingt-un" (3+ items)
		- 77 or "soixante-dix-sept" (3+ items)
		- 5001 or "cinquante mille et un" (3+ items)
		- 3,14 (decimal)
