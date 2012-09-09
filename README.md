uabeamertemplate
================

A nice .tex template for people using Nico Schlömer's uabeamer latex beamer style.

This assumes that if you have the fontspec package, you'll also have the Underware Auto1 font. 
If you do have the Auto1 font, be sure to compile with XeTeX or LuaLaTeX. If not, just delete 

    % the official UA font:
    \IfFileExists{fontspec.sty}{
    \usepackage{fontspec}
    \fontspec[Ligatures=TeX]{auto1}
    \setsansfont[Ligatures=TeX]{auto1}
    }
    
and be sad about how your font sucks. 

Commands and Environments
-------------------------
Some notable commands:

    \coloremph{text}

is like \emph{text} but with color.

    \begin{description*}
      \item{text} explanation
	  \item{t2} more explanation
    \end{description*}

can be used instead of description (useful for longer labels). 
