# Overview

A [scriptorium](https://github.com/jasedit/scriptorium) template for writing a resume or cirriculum vitae, based on the [moderncv](http://www.ctan.org/tex-archive/macros/latex/contrib/moderncv/) template. **NOTE**: Currently, the majority of commands provided by the moderncv package cannot be exposed directly in MultiMarkdown, requiring dropping into raw LaTeX for most of these commands. Please see the moderncv examples provided in the package for these commands.

# Instructions

Assuming that scriptorium has been installed, this template can be installed using:
```
scriptorium template -i https://github.com/jasedit/resume.git
```

A new resume can be generated in the folder `$paper` using this template by executing:
```
scriptorium new -t resume $paper
```

# Template Variables

Variables have two potential configuration points, which will be described here. The first point is the frontmatter variable name, which is used by the underlying system to identify the value at build time. The second point is the placeholder value, which can be replaced during the new command, or manually edited later. For the following description, variables will be named in the format `Variable Name, Placeholder Name - Description`

## MultiMarkdown Frontmatter
1. `latex author`,`$AUTHOR` - name of the paper author
2. `latex title`, `$TITLE` - title of the document, either "Resume" or "Cirriculum Vitae"
3. `my abstract`, `$ABSTRACT` - defines the name of the file to include directly into the LaTeX output as the quote or mission statement at the start of the resume.
4. `bibtex`, `$BIBTEX` - defines the Bibtex file to process for this document. Delete this line to eliminate bibliography support
5. `my style`, `$MYSTYLE` - defines the resume style in use, and must be one of: 'casual', 'classic', 'oldstyle', 'banking' (default)
6. `my color`, `$MYCOLOR` - defines the thematic color of the document, must be one of: 'blue' (default), 'orange', 'green', 'red', 'purple', 'grey', or 'black'
7. `my address`, `$MYADDRESS` - Optional address to include at top of resume.
8. `my mobile`, `$MYMOBILE` - Optional mobile phone number
9. `my fixed`, `$MYFIXED` - Optional fixed (e.g. landline) phone number
10. `my fax` - Optional fax number
11. `my email`, `$MYEMAIL` - Optional email address
12. `my linkedin`, `$MYLINKEDIN` - Optional [LinkedIn](https://www.linkedin.com/) account name.
13. `my twitter` - Optional [Twitter](twitter.com) handle
14. `my github`, `$MYGITHUB` - Optional [Github](https://github.com) account name
15. `my extra info` - Optional extra info string.
16. `my photo` - Optional photo location
9. `mypackages` - If defined, includes the value of this key as a filename in the document preamble, allowing for custom packages and commands to be included
