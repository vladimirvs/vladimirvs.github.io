---
layout: post
title: "Installing Jekyll to Github Pages"
date: 2020-02-03 21:55:42 +0000
categories: jekyll
comment_issue_id: 1
---

I am new to both Ruby and Jekyll. Also to Github Pages. Here's a short guide for people like me who want
to install their own simple static blog without too much fuss!

1. Install Jekyll: [Jekyll installation](https://jekyllrb.com/docs/installation/#guides){:target="\_blank"}
2. Create your GitHub Pages page : [GitHub Pages guide](https://guides.github.com/features/pages/#setup){:target="\_blank"} (follow up to the point where they start talking about choosing a theme - you won't need that). Make sure to name your repo: **yourname.github.io**
3. Make sure you have git installed on your machine: [Git Installation](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git){:target="\_blank"} (just select your OS and download the installer).
4. Having git installed open a new terminal (or cmd.exe) and make sure to check that git is installed:
   `git --version`
5. Clone your repo that you created in step `2` by logging to GitHub and going to your newly reated repo and copying the repo URL:  
   ![My helpful screenshot](/assets/clone-from-github.PNG)

   And then by typing the below command along with the copied URL into your terminal:
   `git clone https://github.com/vladimirvs/vladimirvs.github.io.git`

6. Next go to the newly created folder (in this case `vladimirvs.github.io`) and type:

   `jekyll new .`

7. `jekyll build`
8. You can do `jekyll serve` to see it locally (then open localhost:4000)
9. Commit and push to GitHub:
   `git status`
   `git add .`
   `git commit`
   `git push`
10. If all OK, open your newly created site on `yourusername.github.io` (wait for 1 minute or 2)

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]: https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
