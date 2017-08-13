# org-tikzcd-snippet
A snippet to quickly create and insert Tikz commutative diagrams in org-publish


Usage
-----
MathJax does not regconize tikz-cd blocs while the math notes that I maintain uses them alot. So I use this snippet to export latex to a PNG file and insert it in the buffer.

1. Write a tikz-cd diagram inside a org-mode src bloc.
2. Execute the code (by default with C-c C-c).
3. Copy the link under #+RESULT header to the image bloc under it. 

Notices
--------------
 - PNG files are stored as ../img/[YYY-MM-DD]file.png
 - To ignore the warning, add 
 
         (add-to-list 'warning-suppress-types '(yasnippet backquote-change)) 
     
   to .emacs file 
 
