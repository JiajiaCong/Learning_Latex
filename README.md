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
