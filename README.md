# Git Mastering

## The Four Areas

- Stash
- Working Area
- Staging Area or Index
- Repository

## Git Dif

```
git diff # comparing Working Area <---> Index
git diff --cached # comparing Index <---> Repository
git diff HEAD # comparing Working Area <---> Repository
git diff {commit nummber} {commit number or HEAD} # comparing between commit
```

## Git add & Git rm

```
git add somethink # add somethink to Index

git rm --cached somethink # delete on Index // soft delete
git rm somethink # delete on Working Area and Index // hard delelete
```

## Git checkout

```
git checkout somethink<branch> # move all file from Repository to Index & Working Area
```

## Git Commit

```
git commit -m "comment" # move somethink on Index to Repository
```

## Git reset

```
git reset --hard {commit number} # ย้ายไปจุด commit ที่เลือก และ copy all from Repository to Index & Working Area
git reset --mixed {commit number} # ย้ายไปจุด commit ที่เลือก และ copy all from Repository to Index
git reset --soft {commit number} # ย้ายไปจุด commit ไปที่ Repository

git reset HEAD # copy all from Repository to Index เป็นการทำให้ไฟล์ใน Index เท่ากันกับ Repository
git reset --hard HEAD # copy all from Repository to Index เป็นการทำให้ไฟล์ใน Index, Working เท่ากันกับ Repository

// Trick
git checkout HEAD somethink # เป็นการทำให้เฉพาะไฟล์ somethink กลับมาเท่ากัน Repositoy, Index, Working Area
git checkout -- somethink # shot hand
```

## Git stash

```
git stash --include-unstracked # ย้ายของที่ modify และ add เข้า index ไปแล้ว ไปไว้ที่ stash
git stash list
git stash apply
git stash clear
```

## Git log

```
git log --graph --decorate --oneline
```

## Git show

```
git show HEAD^^ # แสดง commit ถัดไป 2 commit นับจาก HEAD
git show HEAD~2 # แสดง commit ถัดไป 2 commit นับจาก HEAD
git show HEAD@{"1 month ago"}
```

## Git merge <Automatic Merge>

```
git merge <branch> -m "comment"
```

## Git rebase

## Git revert

## Git cherry-pick
