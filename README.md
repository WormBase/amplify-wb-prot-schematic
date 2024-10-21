# amplify-wb-protein-schematic

Repo to drive AWS Amplify builds for the protein browser

Updating for new releases is generally very easy if you don't need to update
the underlying JBrowse 1 software (which you probably don't). All that should
be needed is something like:

```
cd amplify-wb-prot-schematic/data
git checkout staging
perl -pi -e 's/WS292/WS293/' */trackList.json
git add */trackList.json
git commit
git push
```

of course, updated for previous and new release versions.
