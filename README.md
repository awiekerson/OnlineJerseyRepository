
Publish React App to Github pages:

Go into 'package.json
1. Add  "homepage": "https://awiekerson.github.io/[repository name]", to the first line of the file
2. Add  "predeploy": "npm run build", and "deploy": "gh-pages -d [build folder name]", under the scripts section
3. If using vite - add   base: '/[repositoryname]/', to the top od 'defineConfig

Then push to github:

1. git add *
2. git commit -m "message"
3. git push

Check for changes in github repository: 

1. run npm run build
2. run npm run deploy - See if final message says "published"

The app should be running in github pages! 
