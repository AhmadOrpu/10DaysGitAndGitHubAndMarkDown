git -v (to check the current  git version)

To check the current user name and email=>

git config --get user.name Or git config user.name
git config --get user.email Or git config user.email

To set user and email =>

git config --global user.name "Ahmad Sahel" 
git config --global user.email "ahmadorpu95@gmail.com"


// All Commands --------------------------------

Working Directory => Stage Directory => Local Directory => Remote Directory



// git initialization
ls         =>(all files in the working directory check korte)
ls -a      =>(hidden files in the working directory check korte)
git init   =>(git initialization korte)
cd .git , ls   =>(cd .git kore git er hidden files golo dekhte parbo)


cd ../                       =>(cd ../ diye agger main folder e back kora)
touch test.text              =>(to create a test file)
rm -rf abcd.txt              =>(rm -rf abcd.txt to remove a file)
open test.txt   =>(to check what information inside the test file)q                           =>(ripple theke ber hoye terminal e back kora)
git status                   =>(git status diye stage e ki ki ase oita dekha)
git add test.txt             =>(to track the changes in the test file)
git commit -m "added one line in test.txt"   => ( to commit your changes)
git log       =>( to check the changes history )
git log --oneline  =>( to see the logs in shortly )

git reset --hard commitID   =>( to move 1 log to another /commit to another)
git reflog     =>( to see the details what i have done and moves i did )
git rm --cached talk.js    =>( to unstage/untrack the staged/tracked file)
git rm talk.js =>( to delete/remove the staged/tracked file permanently)

touch .gitignore =>( to create a new .gitignore and inside the .gitignore file write the files what you want that git ignore)
git add .gitignore
git commit -m "added .gitignore file"

//Branching
git branch 
git branch feature1
git switch feature1

git branch feature2
git switch feature2

git switch feature1
git switch master =>(cz master branch er sathe feature1 branch mergekorbo)
git merge feature1 


git switch feature2
git switch master =>(cz master branch er sathe feature2 branch mergekorbo)
git merge feature2 =>( now git conflict korbe)

git add test.txt
git commit -m "resolved git conflict issue"


git switch feature1
git branch -m development =>( branch name feature1 rename development) 

git branch -d feature2 =>(branch softly delete korte , mane branch e jode amn kiso thake apni commit koren nei tahole reminder dibe );

git branch -D feature2 =>(branch permanently delete korte)


//Stash(mane holo kono file e kiso edit kore ami atpresent chacesse na git add and commmit korte cz ay file e r o onk kaj korte hobe, tokhn ami stashing korte pari mane holo hide kore rakhte pari . aita kora chara branch switch kora jabe na error dibe)

git stash 
git stash -a       =>(multiple file stash korte)
git stash list     =>(ki ki stash kora ache check korte)
git stash show -p  =>(ki ki stash kora chilo aita dekhabe)
git stash pop      =>(stash ta k fireye ante)
git stash clear    =>(stash ta jode dorker na hoi clear kore dite pari )










