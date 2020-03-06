# MorphologicalDisambiguation

Morphological disambiguation is the problem of selecting accurate morphological parse of a word given its possible parses. These parses are generated by a morphological analyzer. In morphologically rich languages like Turkish, the number of possible parses for a given word is generally more than one. Each parse is considered as a different interpretation of a single word. Each interpretation consists of a root word and sequence of inflectional and derivational suffixes. The following table illustrates different interpretations of the word ‘‘üzerine’’.

üzer+Noun+A3sg+P3sg+Dat  
üzer+Noun+A3sg+P2sg+Dat  
üz+Verb+Pos+Aor+^DB+Adj+Zero+^DB+Noun+Zero+A3sg+P3sg+Dat  
üz+Verb+Pos+Aor+^DB+Adj+Zero+^DB+Noun+Zero+A3sg+P2sg+Dat

As seen above, the first two parses share the same root but different suffix sequences. Similarly, the last two parses also share the same root, however sequence of morphemes are different. Given a parse such as

üz+Verb+Pos+Aor+^DB+Adj+Zero+^DB+Noun+Zero+A3sg+P3sg+Dat

each item is separated by ‘‘+’’ is a morphological feature such as Pos or Aor. Inflectional groups are identified as sequence of morphological features separated by derivational boundaries ^DB. The sequence of inflectional groups forms the term tag. Root word plus tag is named as word form.  So, a word form is defined as follows:

IGroot+IG<sub>1</sub>+^DB+IG<sub>2</sub>+^DB+...+^DB+IG<sub>n</sub>

Then the morphological disambiguation problem can be defined as follows: For a given sentence represented by a sequence of words W = w<sub>1</sub><sup>n</sup> = w<sub>1</sub>, w<sub>2</sub>, ..., w<sub>n</sub>, determine the sequence of parses T = t<sub>1</sub><sup>n</sup> = t<sub>1</sub>, t<sub>2</sub>, ..., t<sub>n</sub>; where t<sub>i</sub> represents the correct parse of the word w<sub>i</sub>.

For Developers
============
You can also see either [Python](https://github.com/olcaytaner/TurkishMorphologicalDisambiguation-Py) 
or [Java](https://github.com/olcaytaner/TurkishMorphologicalDisambiguation) repository.

## Requirements

* [C++ Compiler](#cpp)
* [Git](#git)


### CPP
To check if you have compatible C++ Compiler installed,
* Open CLion IDE 
* Preferences >Build,Execution,Deployment > Toolchain  

### Git

Install the [latest version of Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

## Download Code

In order to work on code, create a fork from GitHub page. 
Use Git for cloning the code to your local or below line for Ubuntu:

	git clone <your-fork-git-link>

A directory called TurkishMorphologicalDisambiguation-CPP will be created. Or you can use below link for exploring the code:

	git clone https://github.com/olcaytaner/TurkishMorphologicalDisambiguation-CPP.git

## Open project with CLion IDE

To import projects from Git with version control:

* Open CLion IDE , select Get From Version Control.

* In the Import window, click URL tab and paste github URL.

* Click open as Project.

Result: The imported project is listed in the Project Explorer view and files are loaded.


## Compile

**From IDE**

After being done with the downloading and opening project, select **Build Project** option from **Build** menu.
