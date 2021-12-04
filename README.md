# VimGolf 문제 풀기

**문제 1. Add quotes to ansible playbook**

![제목 없음1](https://user-images.githubusercontent.com/94671864/144715277-10d1cfc2-8c2c-4c89-81a8-2d7ce3def53a.png)

*******

* 나의 풀이 (score : 9 | highest score : 8)

```
GWi"<End>"<Esc>ZZ
```
`G` : 파일의 마지막 줄로 이동

`W` : 한 라인에서 의미상 다음단어의 시작으로 이동

`i` : 현재 위치에서 입력 모드 시작

여기까지 수정할 위치를 찾아서 갔고

`"` 을 입력해 추가

`<End>` : 라인 끝으로 이동 (`$` 을 사용하려면 `<Esc>` 를 눌러야지만 사용되어서 명령어 수를 줄이기 위해 `<End>` 키 사용)

`"` 을 입력해 추가

`<Esc>` : 입력 종료

`ZZ` : 저장 후 종료 (`:wq` 를 사용하면 명령어 수 증가)

![ezgif com-gif-maker](https://user-images.githubusercontent.com/94671864/144715383-ed9e6106-cf30-4119-a3bb-a77dd7747412.gif)

*********

**문제 2. simple replacement (score : 27 | highest score : 19)**

![제목 없음2](https://user-images.githubusercontent.com/94671864/144716178-a0389623-743b-48ce-a458-4c4f231c5891.png)

******

* 나의 풀이

```
:%s/sublime\|emacs/vim/g<CR>ZZ
```
`:%s/str/replace/g` : str을 replacse로 치환한다.

`\|` 을 이용해 치환 문을 두번 사용하지 않게 하였다. sublime과 emacs는 둘 다 vim으로 치환할 것이기 때문에 하나의 명령으로 치환시켰다.

`<CR>` : Enter키

`ZZ` : 저장 후 종료

![ezgif com-gif-maker (1)](https://user-images.githubusercontent.com/94671864/144716298-af72556e-c0ef-4d57-8db8-fcf5405f14cc.gif)

*********

**문제 3. Satisfy the go linter (score : 33 | highest score : 20)**

![제목 없음3](https://user-images.githubusercontent.com/94671864/144717515-eccbfb7f-f249-42c0-925a-85e61432ffbe.png)

******

* 나의 풀이

```
4GO// Version TODO<Esc>Y<CR>pwcwDebug<Esc>ZZ
```
`4G` : 4번째 줄로 이동한다.

`O` : 현재 라인을 다음 줄로 밀고 입력한다.

`// Version TODO` : 추가할 문장 입력

`<Esc>` : 입력 종료

`Y` : 현재 라인 전체 복사

`<CR>` : 엔터키를 통해 아래 줄로 이동

`p` : 현재 줄을 다음 줄로 밀고 복사한 내용 붙여넣기

`w` : 단어 시작 위치로 이동

`cw` : 단어 삭제 후 삽입

`Debug` : 삽입 내용 입력

`<Esc>` : 입력 종료

`ZZ` : 저장 후 종료

![ezgif com-gif-maker (3)](https://user-images.githubusercontent.com/94671864/144717740-0b92565b-3453-4a98-926c-8f32a25482df.gif)



