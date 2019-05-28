# vim-study
Resources for vim study

## Delete 
`x` : 한 글자만 지울때 

`dw` : 한 단어를 끝까지 지우려면
`d$` : 그 줄 끝까지 지워집니다.

### [횟수]   d   대상      또는      d   [횟수]   대상
- 횟수 - 명령을 몇 번 수행할 지 (옵션, 기본값=1).
- d    - 지우는 명령
- 대상 - 아래에 제시된 대상에 대해 명령을 수행

적용 가능한 대상의 종류:
  
- w - 커서에서 그 단어의 끝까지 (공백 포함.)
- e - 커서에서 그 단어의 끝까지 (공백을 포함하지 않음.)
- $ - 커서에서 그 줄의 끝까지
    
`2dd` 두줄 전제 삭제 

## Undo

`u` : undo for one change
`U` : undo for whole changes in the line 
`ctrl + r` : undo the undo. 다시 실행

## Put
`p` : `dd`로 지운 줄을 커서가 있는 줄에 붙혀 넣음 

## Replace
`r` : 커서 있는 글자를 바꿀 수 있음
