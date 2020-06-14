### Haskell
1. Writing Haskell with Vim  
A simple fix for this is to edit your .vimrc and remove the problematic linters.
```haskell
let g:ale_linters = {
    \   'haskell': ['stack-ghc', 'ghc-mod', 'hlint', 'hdevtools', 'hfmt'],
    \}
```
Becomes:
```haskell
let g:ale_linters ={
      \   'haskell': ['hlint', 'hdevtools', 'hfmt'],
      \}
```
[Monica Lent](https://monicalent.com/blog/2017/11/19/haskell-in-vim/)
