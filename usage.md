---
layout: page
title: Using AnATLyzer
permalink: /usage/
---

## Setting up a transformation

* Create new regular ATL project (if it does not exist yet): File -> New -> ATL Project
* Activate AnATLyzer: Right-click on the project -> Add anATLyzer nature
* Every ATL file in the project will be statically analysed every time it is saved, and errors will be reported in the problem view.
* Do not forget to add the @nsURI or @path annotations at the beginning of the transformation to provide the transformation meta-models.
* It is highly recommended to use the anATLyzer view, which provides more information about the problems in the active transformation, including actions to run the constraint solver, quick fix problems and visualization. To do so, `Window -> Show View -> anATLyzer -> Analysis View`
* Troubleshooting: sometimes you need to run the analysis explicitly. Click on the button with two yellow arrows in the Analysis view. The analysis result that will be shown corresponds to the transformation shown in the editor (if no transformation is actively shown in the editor nothing is analysed).

## Keyboard shortcuts

* CTRL + 1 (cursor over an error): Shows quick fix menu.
* CTRL + 1: Shows quick assist menu with proposals to analyse or refactor the code.
* CTRL + B (over a binding): Show dialog with navigation links to resolving rule.
* CTRL + B (over a rule name): Show dialog with navigation links to bindings resolved by the current rule.

## Additional information

There is some additional information in the Github wiki: [https://github.com/anatlyzer/anatlyzer/wiki](https://github.com/anatlyzer/anatlyzer/wiki) 