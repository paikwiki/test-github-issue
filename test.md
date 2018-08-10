# Test

This doc was made for the test. I made a new project and then applied a remote 
repository which was using for another project. This remote repo already has 
source codes. I wonder if I can commit this repo from new working directory.

## 1st result

```
git push -u origin master
To https://github.com/paikwiki/test-github-issue.git
 ! [rejected]        master -> master (fetch first)
 error: failed to push some refs to 'https://github.com/paikwiki/test-github-issue.git'
 hint: Updates were rejected because the remote contains work that you do
 hint: not have locally. This is usually caused by another repository pushing
 hint: to the same ref. You may want to first integrate the remote changes
 hint: (e.g., 'git pull ...') before pushing again.
 hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```

So, I pushed commits with '--force'. It works, but previous source codes of 
remote repo are gone with it's commit history. I lose codes of mine.

## Conclusion

If, you don't need source codes on remote repo, you can commit from new working 
directory with '--force' tag. It will remove whole codes on remote repo and 
replace with new codes. It's not recommenable. 

Don't do that.

