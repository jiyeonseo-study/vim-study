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

`U` : (Capital U) undo for whole changes in the line 

`ctrl + r` : undo the undo. 다시 실행

## Put
`p` : `dd`로 지운 줄을 커서가 **아래** 줄에 붙혀 넣음 

## Replace
`r` : 커서 있는 글자를 바꿀 수 있음

1. 이전 행동을 취소하려면: u (소문자 u)
한 줄에서 수정한 것을 모두 취소하려면: U (대문자 U)
취소한 것을 다시 실행하려면: CTRL-R

## change(변환)

[횟수] c 대상 또는 c [횟수] 대상

c$ 커서부터 끝까지 

## line

`CTRL-g` : 파일의 상태와 파일 내에서의 현재 위치를 표시

"/private/var/folders/n4/ws_1h7316zb6rjv6_2_tbnqhmll586/T/tutorKb9NOh" line 577 of 81
2 --71%-- col 1

SHIFT-G 는 파일의 끝으로 이동

`줄번호 Shift+g` : 그 줄로 이동

## 외부명령

- `:!ls` 외부에서 ls 치는 결과물을 볼 수 있음.
- Press ENTER or type command to continue 이후 엔터치면 돌아옴

- `:w TEST` 같은 경로에 TEST file 만들기
- 같은 방식으로 지울 수 있음 `:rm TEST`

`:#,# w FILENAME` 파일 일부를 다른 파일로 저장 

`:r TEST` 읽어 들여 합치기 (읽어들인 파일은 커서가 위치한 지점에서부터 놓이게 됩니다.) 

`o` 를 누르면 커서 아래에 줄을 만들고 편집 모드가 됩니다.

`O` 를 누르면 커서 윗 줄을 만들고 편집 모드가 됩니다.

`$` 문장 맨 뒤로 간다 

`a` 커서 바로 뒤에 부터 insert 시작 

`A` 문장 맨 뒤에서부터 insert 시작 

## Search

`/+검색어` : 해당 검색어 알려줌 (앞 → 뒤, 왼쪽 → 오른쪽)

`n` :다음 검색 결과 

`Ctrl+n` : 이전 검색 결과 

 `?+검색어` : 같은 검색 but reverse (뒤→앞, 오른쪽→왼쪽) 

## 괄호 짝 찾기

`(, [, {` 위에 커서 올리고 `%` 하면 짝에 맞는 `), ], }` 로 커서 움직임

다시 % 누르면 원래 앞 커서로 돌아옴 

## 치환

:s/thee/the 를 입력한 후 <ENTER> 를 칩니다. 이 명령은 그 줄에서
처음으로 발견된 것만 바꾼다는 것에 주의하십시오.

s/thee/the/g : ← g(globally) 줄 전체에 적용 (Replace all)

두 줄 사이의 모든 문자열에 대해 치환하려면 다음과 같이 합니다,
:#,#s/old/new/g #,# 는 두 줄의 줄번호를 뜻합니다.
:%s/old/new/g 파일 전체에서 발견된 모든 것을 치환하는 경우입니다.

## replace

`R` 커서부터 해서 뒤에 다 replace 

`r` 한 글자만 replace 

## search setting

`:set ic` 대소문자 구별 안함 

`:set hls is` search 문구 하이라이트 

:`nohlsearch` 하이라이트 없애기 

## vimrc

vim example in Mac ?? 

VIMRUNTIME/vimrc_example.vim 

## Book

- Vim - Vi Improved - by Steve Oualline

[http://iccf-holland.org/click5.html](http://iccf-holland.org/click5.html)

- Learning the Vi Editor - by Linda Lamb

Vimtutor [http://wiki.kldp.org/wiki.php/VimTutorKo](http://wiki.kldp.org/wiki.php/VimTutorKo)
