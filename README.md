# VimGolf 문제 풀기

문제 1. Add quotes to ansible playbook

![제목 없음1](https://user-images.githubusercontent.com/94671864/144715277-10d1cfc2-8c2c-4c89-81a8-2d7ce3def53a.png)

* 나의 풀이

```
GWi"<End>"<Esc>ZZ
```
`G` : 파일의 마지막 줄로 이동

`W` : 한 라인에서 의미상 다음단어의 시작으로 이동

`i` : 현재 위치에서 입력 모드 시작

여기까지 수정할 위치를 찾아서 갔고

`"` 을 입력해 추가

`<End>` :라인 끝으로 이동 (`$` 을 사용하려면 `<Esc>` 를 눌러야지만 사용되어서 명령어 수를 줄이기 위해 `<End>` 키 사용)

`"` 을 입력해 추가

`<Esc>` :입력 종료

`ZZ` :저장 후 종료 (`:wq` 를 사용하면 명령어 수 증가)

![ezgif com-gif-maker](https://user-images.githubusercontent.com/94671864/144715383-ed9e6106-cf30-4119-a3bb-a77dd7747412.gif)


