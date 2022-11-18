---
layout: post
title: Testing markdown
abstract: I test the capabilities of writing markdown posts for this website, including math formatting.
---

The purpose of this post is to test the process of writing a post in markdown, as well as the possibility of embedding code blocks and math equations into the text. Additionally, I also want to evaluate the legibility of my chosen body font, [*IBM Plex Serif*](https://fonts.google.com/specimen/IBM+Plex+Serif).

### Sample paragraph, regular typeface

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus id venenatis ligula. Suspendisse velit tellus, commodo a lobortis sed, suscipit eu sapien. Proin sit amet dictum nisi, nec tristique ligula. Curabitur feugiat elit dui, sed laoreet nunc porttitor quis. Donec vitae iaculis ex. Pellentesque id neque eu quam fringilla mollis. Integer vehicula ante at lacus maximus viverra. Fusce ligula nunc, sodales at ante molestie, faucibus maximus lectus. Nam et convallis ligula. Donec metus velit, venenatis nec accumsan sed, faucibus et leo. Ut elementum mattis enim vel sollicitudin.

### Sample paragraph, italic typeface

In markdown, italics can be selected by surrounding the text with asterisks, like `*[Sample Italic Text]*`.

*Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus id venenatis ligula. Suspendisse velit tellus, commodo a lobortis sed, suscipit eu sapien. Proin sit amet dictum nisi, nec tristique ligula. Curabitur feugiat elit dui, sed laoreet nunc porttitor quis. Donec vitae iaculis ex. Pellentesque id neque eu quam fringilla mollis. Integer vehicula ante at lacus maximus viverra. Fusce ligula nunc, sodales at ante molestie, faucibus maximus lectus. Nam et convallis ligula. Donec metus velit, venenatis nec accumsan sed, faucibus et leo. Ut elementum mattis enim vel sollicitudin.*

### Sample paragraph, bold typeface

Boldface can be selected by surrounding the text with a pair of asterisks, as in `**[Sample Bold Text]**`.

**Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus id venenatis ligula. Suspendisse velit tellus, commodo a lobortis sed, suscipit eu sapien. Proin sit amet dictum nisi, nec tristique ligula. Curabitur feugiat elit dui, sed laoreet nunc porttitor quis. Donec vitae iaculis ex. Pellentesque id neque eu quam fringilla mollis. Integer vehicula ante at lacus maximus viverra. Fusce ligula nunc, sodales at ante molestie, faucibus maximus lectus. Nam et convallis ligula. Donec metus velit, venenatis nec accumsan sed, faucibus et leo. Ut elementum mattis enim vel sollicitudin.**

### Math mode

Inline math can be activated by placing two dollar signs around an equation, like `$$[Insert Inline Equation]$$`. *Note:* this is different from the LaTeX environment, where the double-dollar is a marker for an equation on it's own line! An example of an inline equation is $$f(x)=x^2$$. I am using the mathjax plugin to render these equations. I'm not really sure how it works, I just copyied a forum answer [here](https://talk.jekyllrb.com/t/how-to-use-latex-on-jekyll/4119).

To write out full *centered* equations, use the normal LaTeX block:
```
\begin{equation}
    [Insert Equation]
\end{equation}
```

This is an example, showing the fundamental theorem of calculus:
\begin{equation}
    f(x) = \int^x_0\frac{\mathrm{d}f(x')}{\mathrm{d}x'}\mathrm{d}x' + f(0)
\end{equation}

Another example, more specifically from my field, is the mass-conservation equation for the structure of stars:
\begin{equation}
    \frac{\mathrm{d}M_r}{\mathrm{d}r}=4\pi r^2\rho (r)
\end{equation}

### Code blocks

In the text above, I have used code blocks that look a little like this:
```
program main

INTEGER(kind=16):: n
INTEGER :: step = 1
INTEGER(kind=16):: fact = 2

write(*,*) "Type an integer!"
read(*,*) n

DO WHILE (fact <= SQRT(real(n)))
    IF (MOD(n,fact) == 0) THEN
        write(*,*) fact
        n = n / fact
    ELSE
        fact = fact + step
        step = 2
    END IF
END DO

write(*,*) n
write(*,*)

end program main
```

By the way, the above is Fortran90 code I wrote to compute the prime factors of any integer.

To write a block of code, introduce it with three backticks 
```` 
```
[Insert Code]
``` 
````
Or use a single backtick for inline code, like `` `[Insert Code]` ``.