Learning_Latex
==============

# 数学公式

##数学公式太长要断行

下面的是是对[x+y+z+w+r]进行断行

         \begin{align}   
         h(x)&=x+y\\   
         \begin{split}   
             &=\left[ x+y+z \right.\\   
             &\left. +w+r \right]   
         \end{split}   
         \end{align}   

##数学公式进行编号

align环境中会对每一行都进行编号，有时只想对整个数学式子进行一个编号，或者是对某一行进行编号。可以在不想进行编号的行后面加上\notag。
比如下面的这个例子,在h(x)=x+y这一行后面不加编号。

        \begin{align}
        h(x)&=x+y \notag \\
        \begin{split}
            &=\left[ x+y+z \right.\\
            &\left. +w+r \right]
        \end{split}
        \end{align}

##数学定理

         \documentclass{article}
         \usepackage{times} 
         \usepackage{CJK} 
         \pagestyle{empty} 
         \setcounter{page}{6} 
         \setcounter{section}{5} 
         \setlength\textwidth{151.0pt} 
           \setlength\textheight{.44\textheight}
         \usepackage{amsmath,amssymb} 
         \begin{CJK*}{GBK}{song}  
         \newtheorem{theorem}{{定理}} 
         \newtheorem{proposition}{{命题}} 
         \newtheorem{proposition}{Proposition} 
         \newtheorem{lemma}{{引理}} 
         \newtheorem{lemma}{Lemma} 
         \newtheorem{corollary}{{推论}}[theorem] 
         \newtheorem{definition}{{定义}} 
         \newtheorem{example}{{例}} 
         \begin{document} 
         \section{数学常用环境的汉化} 
         
         \begin{definition} 
           定义的例子。
         \end{definition} 

         \begin{lemma} 
           引理的例子。
         \end{lemma} 
         
         \begin{theorem} 
           定理的例子。
         \end{theorem} 
         
         \begin{lemma} 
           第二个引理的例子。
         \end{lemma} 
         
         \begin{theorem} 
           第二个定理的例子。
         \end{theorem} 
         
         \begin{corollary} 
           推论的例子。
         \end{corollary} 

         \begin{corollary} 
           第二个推论的例子。
         \end{corollary} 
         
         \begin{proposition} 
           命题的例子。
         \end{proposition} 
         
         \begin{example} 
           例的例子。
         \end{example} 
         
         \end{CJK*} 
         \end{document}
