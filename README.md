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

![6KvKomiJ0T](https://user-images.githubusercontent.com/94671864/144739819-34123495-d2e8-4dd4-923f-1c7a4d8c8a77.gif)


*********

**문제 4. Plotting some variables in python (score : 59| highest score : 34)**

![제목 없음1](https://user-images.githubusercontent.com/94671864/144740050-96ac4133-f084-4f9b-9b67-723adc532f29.png)

******

* 나의 풀이

```
:%s/y1/abs(y1)/g<CR>:s/1/4/g<CR>:4s/1/3/g<CR>:3s/1/2/g<CR>fksb<Down><BS>r<Down><BS>g<Esc>ZZ
```
`:%s/y1/abs(y1)/g` : y1을 모두 abs(y1)으로 치환

`:s/1/4/g` : 현재 라인에 있는 1을 모두 4로 치환

`:4s/1/3/g` : 4 라인에 있는 1을 모두 3으로 치환

`:3s/1/2/g` : 3 라인에 있는 1을 모두 2으로 치환

`fk` : 커서를 k앞으로 이동

`s` : 커서 뒤 단어 삭제

이후 `b`로 변경, 커서를 아래로 내리면서 r, g로 바꿈

`<Esc>` : 입력 종료

`ZZ` : 저장 후 종료

![kDfm0QgKjI](https://user-images.githubusercontent.com/94671864/144740002-15007df2-57bc-4f54-ad42-d40f46da2526.gif)

*********

**문제 5. Python dataclasses (score : 32| highest score : 19)**

![제목 없음2](https://user-images.githubusercontent.com/94671864/144746235-dd6a53ac-b5a8-419d-9ded-28900291a4b5.png)

******

* 나의 풀이

```
/"<CR>astudent_id,name,age,score<Esc>ZZ
```
`/"` : **"** 찾기

`a` : 현재 커서 뒤에서 부터 삽입

`student_id,name,age,score` : 삽입 내용

`<Esc>` : 입력 종료

`ZZ` : 저장 후 종료

![hzTrF9HSE7](https://user-images.githubusercontent.com/94671864/144746287-802d772e-9524-45d7-aaaf-7a5e07dec2d8.gif)




