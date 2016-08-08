# test_ipynb
Test sync-ing an ipynb >> md >> latex >> md >> latex cycle
The idea is something like this:

1. Create an overleaf project, add .ipynb, .md 
2. Clone overleaf git
3. cd overleaf_project
4. Clone this git repo
5. cd git_repo
6. jupyter notebook
7. Start a regular notebook with R frontend and compose some markdown formatted text
8. download as markdown file
9. In terminal, use pandoc -f markdown -t latex -o test.tex
10. git add .
11. git commit -m "added tex"
12. git push
13. cd .. (move to overleaf folder)
14. git add .
15. git commit -m "added github folder markdown text and latex"
16. git push 

## What will happen?
- I can work with the flexibility and peace of mind of ipynb notebook
- I can access the ipynb notebook wherever I want
- I can work on the ipynb notebook and push to overleaf
- Overleaf can push it out to the rest of the world as pdf
