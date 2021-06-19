# Minimal React Boilerplate

Quickly setting up small demo pages. No bleeding edge, no complex production sites.

## Set up

With YOUR-PROJECT as path to maintain "Your Project":

```
NEW_PROJECT="YOUR-PROJECT"
git clone --depth=1 https://github.com/hh-lohmann/minimal-react-boilerplate.git "$NEW_PROJECT"
cd "$NEW_PROJECT"
git remote remove origin
npm i
echo '/output' > .gitignore
git add .
git commit --amend -m 'Boilerplate from https://github.com/hh-lohmann/minimal-react-boilerplate' --author="$(git config user.name) <$(git config user.email)>" --date="$(date)"

```
(You can set `NEW_PROJECT="YOUR-PROJECT"` at command line and then copy the rest in one bunch from here and paste into your terminal, each command will find its line, the last one might need an explicit Return key press)

This gives you a fresh project directory with Git version control for your data instead of that of the boilerplate, including the "node_modules" dir for some possible disaster recovery. Leave out the lines between "npm " and "git commit" if you don't want to track the state of the "node_modules" dir.



## Develop project

```

npm run dev

```

This should automatically open your browser with `http://localhost:9000`, if not, launch this address by hand.



## Build a Production Bundle

```

npm run build

```

Bundle is built as "bundle.min.js" in directory "output" of "YOUR-PROJECT", "output" is created if not existing yet.

You can test this bundle by opening `index.html` in a browser.


