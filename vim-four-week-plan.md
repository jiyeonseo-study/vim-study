# Vim 정복하기: 4주 계획 How To Learn Vim: A Four Week Plan

참고 : [English Blog](https://medium.com/actualize-network/how-to-learn-vim-a-four-week-plan-cd8b376a9b85),  
 [한국어 블로그 글](https://medium.com/@jungseobshin/vim-%EB%B0%B0%EC%9A%B0%EB%8A%94-%EB%B2%95-4%EC%A3%BC-%EA%B3%84%ED%9A%8D-77f3f7e263f7)

## Week 1: 
vimtutor 하루에 한 번, 매일 끝까지 실습하기 
Complete vimtutor once a day, every day

```
$ vimtutor
$ vimtutor ko
```

- [x] Week 1, Day 1
### w b e
- w : 전 단어의 맨 앞으로 커서 이동
- b : 뒤 단어의 맨 앞으로 커서 이동 
- e : 해당 단어, 다음 단어 마지막 글자로 커서 이동 

### Why vim uses hjkl as arraw keys + esc 
https://catonmat.net/why-vim-uses-hjkl-as-arrow-keys

### simple tips 
- vim 에디터로 시작하지 마시고, 익숙한 IDE의 vim 플러그인으로 시작하세요. 

### avoid esc key 
https://vim.fandom.com/wiki/Avoid_the_escape_key 

### basic cheat sheet
![](vi-vim-tutorial-1.gif)
reference : [http://www.viemu.com/a_vi_vim_graphical_cheat_sheet_tutorial.html](http://www.viemu.com/a_vi_vim_graphical_cheat_sheet_tutorial.html)

- [x] Week 1, Day 2

## 0 (Zero)
Type  0  (zero) to move to the start of the line.

### G gg
- Press  G  to move you to the bottom of the file.
- Type  gg  to move you to the start of the file.

### go back after searching(`/` or `?`)
- To go back to where you came from press  CTRL-O 
- Repeat to go back further.
- CTRL-I goes forward.

### substitute

`:%s/old/new/gc` : 바뀌는 모든 문자열 찾은 다음에 바꿀껀지 물어봄. 
To ask for confirmation each time add 'c'

### Visual 

- `v` and move consor 문장 선택하기
- Press the  :  character.  At the bottom of the screen  :'<,'> will appear.

- `y` : yank (copy) 
- `p` : paste 

- [x] Week 1, Day 3

## Chrome extension 
- Vimium https://vimium.github.io/

- [x] Week 1, Day 4

## Vim adventure 
- https://vim-adventures.com/

- [ ] Week 1, Day 5
- [x] Week 1, Day 6

## PR for updaring vimtutor ko
- https://github.com/vim/vim/pull/4503

- [x] Week 1, Day 7

## blog 
- https://jiyeonseo.github.io/2019/06/07/vim-study-week1/

## Week 2: 
최소한의 설정, 플러그인 없이 Vim 사용하기
Use Vim with minimal config, no plugins

- [x] Week 2, Day 1

ref : https://dougblack.io/words/a-good-vimrc.html#spaces 

## .vimrc
> Don't put any lines in your vimrc that you don't understand.

## rimrc_example.vim
https://github.com/vim/vim/blob/314dd79cac2adc10304212d1980d23ecf6782cfc/runtime/vimrc_example.vim

## Colors 
```
syntax enable
```
## Spaces & Tabs 
```
set tabstop=4
```
the number of spaces a tab counts for. So, when Vim opens a file and reads a <TAB> character, it uses that many spaces to visually show the <TAB>.

```
set softtabstop=4
```
the number of spaces a tab counts for when editing. So this value is the number of spaces that is inserted when you hit <TAB> and also the number of spaces that are removed when you backspace.

## UI Config 
```
set number " show line numbers 
set showcmd " commend in bottom bar
set cursorline " highlight current line
set showmatch " highlight matching [{()}]
```
```
set lazyredraw
```
- for macro? 

## Searching
```
set incsearch   " search as characters are entered
set hlsearch
```



- [ ] Week 2, Day 2
- [ ] Week 2, Day 3
- [ ] Week 2, Day 4
- [ ] Week 2, Day 5
- [ ] Week 2, Day 6
- [ ] Week 2, Day 7

## Week 3:
최소한의 플러그인으로 Vim 사용하기
Use Vim with minimal plugins

- [ ] Week 3, Day 1
- [ ] Week 3, Day 2
- [ ] Week 3, Day 3
- [ ] Week 3, Day 4
- [ ] Week 3, Day 5
- [ ] Week 3, Day 6
- [ ] Week 3, Day 7

## Week 4:
동사와 명사를 활용한 Vim 명령어 사용
Compose Vim commands with verbs and nouns

- [ ] Week 4, Day 1
- [ ] Week 4, Day 2
- [ ] Week 4, Day 3
- [ ] Week 4, Day 4
- [ ] Week 4, Day 5
- [ ] Week 4, Day 6
- [ ] Week 4, Day 7

