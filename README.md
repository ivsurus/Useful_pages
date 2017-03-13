# Useful_pages
GIT COMMENTS https://chris.beams.io/posts/git-commit/
The seven rules of a great Git commit message

1)Separate subject from body with a blank line
2)Limit the subject line to 50 characters
3)Capitalize the subject line
4)Do not end the subject line with a period
5)Use the imperative mood in the subject line
6)Wrap the body at 72 characters
7)Use the body to explain what and why vs. how



How do I clone a subdirectory only of a Git repository
http://stackoverflow.com/questions/600079/how-do-i-clone-a-subdirectory-only-of-a-git-repository
mkdir <repo>
cd <repo>
git init
git remote add -f origin <url>
git config core.sparseCheckout true
echo "pom.xml" >> .git/info/sparse-checkout
echo "src" >> .git/info/sparse-checkout
git pull origin master
