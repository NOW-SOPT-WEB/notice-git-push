# 🌱 웹파트 Github로 과제를 제출해봅시다 🌱

## 1️⃣ Github Organiztion 방문

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/a3b89dc5-3039-4ea6-a1f4-4d4ded7922df)

---

## 2️⃣ 내 Repository 찾기

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/5330b4ef-870a-4526-bc43-cb50c42e58f2)




---

## 3️⃣ 클론할 url 복사하기
![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/3a017d2b-4096-48fb-8713-0fbfd3ba8f6f)
![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/97244a93-7045-47b8-ba16-4608d11e9fe2)



---

## 4️⃣ 터미널, cmd를 열고, 내가 프로젝트를 관리할 디렉토리(폴더)로 이동한다.
저는 VSCode에서 `Open Folder`로 프로젝트를 관리하고자 하는 디렉토리를 열어주고, 거기서 터미널을 열었습니다!

ex) VSCode open folder

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/2c45e850-e2ff-490c-afd9-967b41a036ef)

ex) terminal 디렉토리 이동

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/05d31082-6fa1-4312-87fb-807dd08e934b)


---

## 5️⃣ Repository Clone 하기.

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/3fa13c02-5e39-4df9-81e1-dd2bcd6d72c0)


```bash
git clone {아까 복사한 url}
```

~~중괄호는 넣는거 아닙니다!~~

```
🌱 remote: ~~~ done 이라 나오면, clone이 완료된 거랍니다. 
그럼 여러분의 repository의 이름으로 폴더가 생성될 거에요.

이동해봅시다.
```
![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/300bb2d7-edad-447c-ab49-f5613db73161)


```
🌱 이 디렉토리는 이제 git이 활성화 된 디렉토리가 됐어요.
여러분의 경우에는 해당 디렉토리 안에 ``README 파일``이 있을 거에요!

(ls는 디렉토리 내용을 보여주는 리눅스 명령어로 윈도우에선 사용하지 못해요! 지금 단계에선 ls를 사용하지 않아도 무방합니다)
```

---

## 6️⃣ 브랜치 생성하기

브랜치는 작업환경을 분리해주는 친구에요.

우리는 매주 과제마다 브랜치를 생성할거에요.git 

1주차 과제를 진행한다고 가정하고 `week1` 이라는 브랜치를 만들어봐요.

우선 git이 활성화 되어있는 여러분 레포이름으로 되어있는 디렉토리로 이동해봅시다.

다음 명령어를 통해서 `week1` 브랜치를 생성해보아요.

```bash
git branch week1
```

잘 생성되었을까요?

```bash
git branch
```
![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/4addb7ed-eed2-44fb-a3f7-189ddf59b834)

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/e3bca25a-2467-484d-93a9-6cbda86f9ee0)


위와 같이 week1 브랜치가 나온다면 잘 생성된거에요!

---

## 7️⃣ 생성한 브랜치로 이동하기

브랜치를 만들었으면 해당 브랜치로 이동해야겠죠?

다음 명령어를 사용해서 이동해봅시다.

```bash
git checkout week1
```

week1 브랜치가 정상적으로 생성되지 않았다면 에러가 발생할거에요!

- 생성과 이동을 한 번에 하는 명령어
    
    ```bash
    git checkout -b week1
    ```
    

git branch 명령어로 잘 이동했는지 볼까요?

```bash
git branch
```

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/d74da461-10b9-45a2-8702-69b1d468132a)

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/1e724322-d1d1-4c27-9ca1-99b11b57b916)



---

## 8️⃣ 생성한 브랜치에서 작업하고 커밋 하기

```bash
git status
```

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/e6b60516-5a25-4d3b-bb46-66dbeff97a51)

![image](https://github.com/DO-SOPT-WEB/notice-git-push/assets/97084864/1f6af93a-ed82-45c6-96ec-e115eab1b659)


변경사항이 없다고, `working tree` 가 깨끗하다네요!

이 브랜치에서 과제를 수행한다고 가정해볼게요.

`week1` 폴더 안에 `index.html` 파일을 생성했다고 가정해보죠.

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/4bc7c164-bfaa-4f7a-97ff-467d8eeab0f6)

다시 현재 상태를 확인해봅시다! 

```bash
git status
```

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/de928198-84ac-4c84-9865-563f7b05fa6f)

추적중이지 않은 `week1` 이 있다고 말해주고 있네요.

한 번 야무지게 추적해봅시다.

```bash
git add .
```

```
🌈  "." 이 의미하는 것은 전체에요. 
추적 중이지 않은 "모든 파일"을 추적하겠다는 뜻이 되겠네요. 추적한 이후로는 파일의 변경점을 git으로 확인할 수 있어요!
```


```
🌈 이 단계를 "staging area" 에 있다고 하는데요.
"커밋할 준비가 된 상태"를 의미해요.

커밋을 하기 위해서 우리가 로컬에서 작업한 파일들을 staging area로 올려주는 작업이 필요해요.
이를 위해서 `git add` 명령어가 필요한거랍니다.
```

```
🙋🏻‍♂️ "여기서 커밋이란?"

음 ... 작업한 것에 대한 변경점을 기록한다! 는 의미에요.

작업환경의 현재상태를 사진을 찍어놓는 듯한 ... 스냅샷과 같은 역할을 한답니다.

특정 커밋의 상태로 환경을 돌릴 수도 있고.
커밋 단위로 어떤 작업을 했는지 확인할 수도 있어요.

Git을 사용하는데 있어 가장 중요한 역할을 해요.

그렇기 때문에
"커밋의 단위"를 잘 나누는 것이 중요해요!

모든 과제를 완료할 때까지 한 번도 커밋을 하지 않다가 모두 완성하고 커밋을 한다면?

작업환경의 기록은 딱 두가지로 나뉘겠죠.
과제를 완성하기 전과 후! 

커밋 단위를 잘 나누는 습관을 들여봅시다 우리!
```

그럼 한 번 커밋을 작성해봅시다.

```bash
git commit -m "커밋 메시지를 여기에 입력하세요."
```

```
🌈  커밋 메시지는 아무렇게나 입력해도 되지만...
❌❌❌❌ 아무렇게나 입력하면 안됩니다! ❌❌❌❌

팀을 위해, 협업을 위해 "내가 무슨 작업을 했는 지"를 알아볼 수 있도록 작성하는게 좋아요.
이런 커밋의 룰을 팀끼리 정하는 경우가 있는데 이를 `커밋 컨벤션` 이라고 해요.

이후 합동 세미나나, 솝커톤, 앱잼 등에서 팀마다의 컨벤션을 정하고 진행하게 될 것이에요
```

커밋이 성공적으로 완료되었고 더 이상 커밋할 것이 없다고 말해주고 있네요.

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/286f59ab-f86b-44e7-b92d-a92e014ec5d7)

```bash
git status 는 git의 상태를 보기 위한 명령어로 이해를 돕기위해 작성했을 뿐 필수가 아닙니다!
```

## 9️⃣ 로컬 커밋을 Github로 Push하기

마지막 단계까지 왔네요.

커밋은 성공적으로 완료했지만 이는 아직 Github에는 반영되지 않았을거에요.

아직 내 작업환경에 대한 스냅샷을 가지고 있을 뿐 이를 깃허브에 보내지 않은 상태! 라고 이해하시면 되겠네요.

이제 이를 다른 사람도 확인할 수 있도록 ***Push*** 하는 작업을 해볼게요.

다음의 명령어를 실행해보아요.

```bash
git push origin week1
```

`origin이라는 이름을 갖는 remote 저장소에 week1 브랜치에서 작업한 변경점을 보내겠다` 라는 의미가 되겠네요.

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/8fafc02c-0967-49c6-a751-47974ddefa1e)

성공적으로 push가 완료되었다면 Github 상에서 내가 작업한 변경점을 확인할 수 있게 될 거에요!

![image](https://github.com/NOW-SOPT-WEB/notice-git-push/assets/81609304/edf35fdb-1145-4484-ae7c-48a214b4ee61)

---

**전체적인 그림은 다음과 같아요**

![image](https://user-images.githubusercontent.com/47105088/192493167-1890ac87-5c7c-4ec1-93e6-549631b98be3.png)

